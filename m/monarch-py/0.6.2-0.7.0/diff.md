# Comparing `tmp/monarch_py-0.6.2.tar.gz` & `tmp/monarch_py-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monarch_py-0.6.2.tar", max compression
+gzip compressed data, was "monarch_py-0.7.0.tar", max compression
```

## Comparing `monarch_py-0.6.2.tar` & `monarch_py-0.7.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0      955 2023-04-19 20:22:07.897810 monarch_py-0.6.2/pyproject.toml
--rw-r--r--   0        0        0       77 2023-04-19 20:22:07.897810 monarch_py-0.6.2/src/monarch_py/__init__.py
--rw-r--r--   0        0        0     5897 2023-04-19 20:22:07.897810 monarch_py-0.6.2/src/monarch_py/cli.py
--rw-r--r--   0        0        0        0 2023-04-19 20:22:07.897810 monarch_py-0.6.2/src/monarch_py/datamodels/__init__.py
--rw-r--r--   0        0        0     6595 2023-04-19 20:22:07.897810 monarch_py-0.6.2/src/monarch_py/datamodels/model.py
--rw-r--r--   0        0        0     6327 2023-04-19 20:22:07.897810 monarch_py-0.6.2/src/monarch_py/datamodels/model.yaml
--rw-r--r--   0        0        0     3300 2023-04-19 20:22:07.897810 monarch_py-0.6.2/src/monarch_py/datamodels/solr.py
--rw-r--r--   0        0        0        0 2023-04-19 20:22:07.897810 monarch_py-0.6.2/src/monarch_py/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 20:22:07.897810 monarch_py-0.6.2/src/monarch_py/implementations/solr/__init__.py
--rw-r--r--   0        0        0    15875 2023-04-19 20:22:07.897810 monarch_py-0.6.2/src/monarch_py/implementations/solr/solr_implementation.py
--rw-r--r--   0        0        0        0 2023-04-19 20:22:07.897810 monarch_py-0.6.2/src/monarch_py/implementations/sql/__init__.py
--rw-r--r--   0        0        0     8913 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/implementations/sql/sql_implementation.py
--rw-r--r--   0        0        0        0 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/interfaces/__init__.py
--rw-r--r--   0        0        0     2345 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/interfaces/association_interface.py
--rw-r--r--   0        0        0      985 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/interfaces/entity_interface.py
--rw-r--r--   0        0        0      890 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/interfaces/query_interface.py
--rw-r--r--   0        0        0     3732 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/interfaces/search_interface.py
--rw-r--r--   0        0        0        0 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/service/__init__.py
--rw-r--r--   0        0        0     2051 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/service/solr_service.py
--rw-r--r--   0        0        0     8269 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/solr_cli.py
--rw-r--r--   0        0        0     3794 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/sql_cli.py
--rw-r--r--   0        0        0        0 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/utils/__init__.py
--rw-r--r--   0        0        0     3657 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/utils/solr_cli_utils.py
--rw-r--r--   0        0        0     4262 2023-04-19 20:22:07.901810 monarch_py-0.6.2/src/monarch_py/utils/utils.py
--rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 monarch_py-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      955 2023-05-03 19:21:04.825506 monarch_py-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-05-03 19:21:04.825506 monarch_py-0.7.0/src/monarch_py/__init__.py
+-rw-r--r--   0        0        0     1587 2023-05-03 19:21:04.825506 monarch_py-0.7.0/src/monarch_py/association_type_mappings.yaml
+-rw-r--r--   0        0        0     6347 2023-05-03 19:21:04.825506 monarch_py-0.7.0/src/monarch_py/cli.py
+-rw-r--r--   0        0        0        0 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/datamodels/__init__.py
+-rw-r--r--   0        0        0     7976 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/datamodels/model.py
+-rw-r--r--   0        0        0     7215 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/datamodels/model.yaml
+-rw-r--r--   0        0        0     3300 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/datamodels/solr.py
+-rw-r--r--   0        0        0        0 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/implementations/solr/__init__.py
+-rw-r--r--   0        0        0    16913 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/implementations/solr/solr_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/implementations/sql/__init__.py
+-rw-r--r--   0        0        0     8909 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/implementations/sql/sql_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/interfaces/__init__.py
+-rw-r--r--   0        0        0     2343 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/interfaces/association_interface.py
+-rw-r--r--   0        0        0      985 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/interfaces/entity_interface.py
+-rw-r--r--   0        0        0      890 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/interfaces/query_interface.py
+-rw-r--r--   0        0        0     3737 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/interfaces/search_interface.py
+-rw-r--r--   0        0        0        0 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/service/__init__.py
+-rw-r--r--   0        0        0     2052 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/service/solr_service.py
+-rw-r--r--   0        0        0     9114 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/solr_cli.py
+-rw-r--r--   0        0        0     3792 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/sql_cli.py
+-rw-r--r--   0        0        0        0 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/utils/__init__.py
+-rw-r--r--   0        0        0     4052 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/utils/association_type_utils.py
+-rw-r--r--   0        0        0     3959 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/utils/solr_cli_utils.py
+-rw-r--r--   0        0        0     4469 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/utils/utils.py
+-rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 monarch_py-0.7.0/PKG-INFO
```

### Comparing `monarch_py-0.6.2/pyproject.toml` & `monarch_py-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monarch-py"
-version = "0.6.2"
+version = "0.7.0"
 description = "Monarch Initiative data access library"
 authors = [
     "Kevin Schaper <kevin@tislab.org>",
     "Glass Elsarboukh <glass@tislab.org>",
     "The Monarch Initiative <info@monarchinitiative.org>"
 ]
 packages = [
```

### Comparing `monarch_py-0.6.2/src/monarch_py/cli.py` & `monarch_py-0.7.0/src/monarch_py/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,17 +37,14 @@
 
 ### "Aliases" for Solr CLI ###
 
 
 @app.command("entity")
 def entity(
     id: str = typer.Argument(None, help="The identifier of the entity to be retrieved"),
-    update: bool = typer.Option(
-        False, "--update", "-u", help="Whether to re-download the Monarch KG"
-    ),
     fmt: str = typer.Option(
         "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
 ):
@@ -68,20 +65,17 @@
     category: str = typer.Option(None, "--category", "-c"),
     subject: str = typer.Option(None, "--subject", "-s"),
     predicate: str = typer.Option(None, "--predicate", "-p"),
     object: str = typer.Option(None, "--object", "-o"),
     entity: str = typer.Option(None, "--entity", "-e"),
     between: str = typer.Option(None, "--between"),
     direct: bool = typer.Option(False, "--direct"),
-    association_label: str = typer.Option(None, "--label"),
+    association_type: str = typer.Option(None, "--label"),
     limit: int = typer.Option(20, "--limit", "-l"),
     offset: int = typer.Option(0, "--offset"),
-    update: bool = typer.Option(
-        False, "--update", "-u", help="Whether to re-download the Monarch KG"
-    ),
     fmt: str = typer.Option(
         "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
 ):
@@ -91,15 +85,15 @@
     Args:
         category: The category of the association
         predicate: The predicate of the association
         subject: The subject of the association
         object: The object of the association
         entity: The subject or object of the association
         between: The subject and object of the association
-        association_label: The label of the association
+        association_type: The label of the association
         limit: The number of associations to return
         direct: Whether to exclude associations with subject/object as ancestors
         offset: The offset of the first association to be retrieved
         fmt: The format of the output (TSV, YAML, JSON)
         output: The path to the output file (stdout if not specified)
     """
     solr_cli.associations(**locals())
@@ -155,17 +149,14 @@
     """
     solr_cli.autocomplete(**locals())
 
 
 @app.command("histopheno")
 def histopheno(
     subject: str = typer.Argument(None, help="The subject of the association"),
-    update: bool = typer.Option(
-        False, "--update", "-u", help="Whether to re-download the Monarch KG"
-    ),
     fmt: str = typer.Option(
         "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
 ):
@@ -178,9 +169,33 @@
     Optional Args:
         fmt (str): The format of the output (TSV, YAML, JSON). Default JSON
         output (str): The path to the output file. Default stdout
     """
     solr_cli.histopheno(**locals())
 
 
+@app.command("association-counts")
+def association_counts(
+    entity: str = typer.Argument(None, help="The entity to get association counts for"),
+    fmt: str = typer.Option(
+        "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
+    ),
+    output: str = typer.Option(
+        None, "--output", "-o", help="The path to the output file"
+    ),
+):
+    """
+    Retrieve association counts for an entity by ID
+
+    Args:
+        entity: The entity to get association counts for
+        fmt: The format of the output (TSV, YAML, JSON). Default JSON
+        output: The path to the output file. Default stdout
+
+    Returns:
+        A list of association counts for the given entity containing association type, label and count
+    """
+    solr_cli.association_counts(**locals())
+
+
 if __name__ == "__main__":
     app()
```

### Comparing `monarch_py-0.6.2/src/monarch_py/datamodels/model.py` & `monarch_py-0.7.0/src/monarch_py/datamodels/model.py`

 * *Files 25% similar despite different names*

```diff
@@ -21,26 +21,26 @@
     underscore_attrs_are_private=True,
     extra="forbid",
     arbitrary_types_allowed=True,
 ):
     pass
 
 
-class AssociationLabel(str, Enum):
+class AssociationTypeEnum(str, Enum):
 
     disease_phenotype = "disease_phenotype"
     gene_phenotype = "gene_phenotype"
     gene_interaction = "gene_interaction"
     gene_pathway = "gene_pathway"
     gene_expression = "gene_expression"
     gene_orthology = "gene_orthology"
     chemical_pathway = "chemical_pathway"
     gene_function = "gene_function"
-    gene_associated_with_disease = "gene_associated_with_disease"
-    gene_affects_risk_for_disease = "gene_affects_risk_for_disease"
+    correlated_gene = "correlated_gene"
+    causal_gene = "causal_gene"
 
 
 class Association(ConfiguredBaseModel):
 
     aggregator_knowledge_source: Optional[List[str]] = Field(default_factory=list)
     id: Optional[str] = Field(None)
     subject: Optional[str] = Field(None)
@@ -163,35 +163,72 @@
 
     label: Optional[str] = Field(None)
     count: Optional[int] = Field(
         None, description="""number of items a this facet value"""
     )
 
 
+class FacetField(ConfiguredBaseModel):
+
+    label: Optional[str] = Field(None)
+    facet_values: Optional[Dict[str, FacetValue]] = Field(default_factory=dict)
+
+
+class AssociationTypeMapping(ConfiguredBaseModel):
+    """
+    A data class to hold the necessary information to produce association type counts for given  entities with appropriate directional labels
+    """
+
+    association_type: Optional[AssociationTypeEnum] = Field(None)
+    subject_label: Optional[str] = Field(
+        None,
+        description="""A label to describe the subjects of the association type as a whole for use in the UI""",
+    )
+    object_label: Optional[str] = Field(
+        None,
+        description="""A label to describe the objects of the association type as a whole for use in the UI""",
+    )
+    category: Optional[List[str]] = Field(
+        default_factory=list,
+        description="""The biolink categories to use in queries for this association type, assuming OR semantics""",
+    )
+    predicate: Optional[List[str]] = Field(
+        default_factory=list,
+        description="""The biolink predicate to use in queries for this association type, assuming OR semantics""",
+    )
+
+
 class AssociationCount(FacetValue):
 
-    id: Optional[str] = Field(None)
+    association_type: Optional[AssociationTypeEnum] = Field(None)
     label: Optional[str] = Field(None)
     count: Optional[int] = Field(
         None, description="""number of items a this facet value"""
     )
 
 
-class FacetField(ConfiguredBaseModel):
+class AssociationCountList(ConfiguredBaseModel):
+    """
+    Container class for a list of association counts
+    """
 
-    label: Optional[str] = Field(None)
-    facet_values: Optional[Dict[str, FacetValue]] = Field(default_factory=dict)
+    items: Optional[List[AssociationCount]] = Field(
+        default_factory=list,
+        description="""A collection of items, with the type to be overriden by slot_usage""",
+    )
 
 
 # Update forward refs
 # see https://pydantic-docs.helpmanual.io/usage/postponed_annotations/
 Association.update_forward_refs()
 Entity.update_forward_refs()
 HistoPheno.update_forward_refs()
 Results.update_forward_refs()
 AssociationResults.update_forward_refs()
 EntityResults.update_forward_refs()
 SearchResult.update_forward_refs()
 SearchResults.update_forward_refs()
 FacetValue.update_forward_refs()
-AssociationCount.update_forward_refs()
 FacetField.update_forward_refs()
+AssociationTypeMapping.update_forward_refs()
+AssociationCount.update_forward_refs()
+AssociationCountList.update_forward_refs()
```

### Comparing `monarch_py-0.6.2/src/monarch_py/datamodels/model.yaml` & `monarch_py-0.7.0/src/monarch_py/datamodels/model.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,17 @@
   linkml: https://w3id.org/linkml/
   biolink: https://w3id.org/biolink/
 description: Data datamodels for the Monarch Initiative data access library
 imports:
 - linkml:types
 default_range: string
 enums:
-  AssociationLabel:
+  AssociationTypeEnum:
     description: >-
-      A grouping label for associations, which are not necessarily 1:1 with
+      A grouping label for association types, which are not necessarily 1:1 with
       biolink categories or predicates
     permissible_values:
       disease_phenotype:
         description: >-
           Any association between a disease and a phenotype
         meaning: biolink:GeneToDiseaseAssociation
       gene_phenotype:
@@ -41,22 +41,21 @@
           description: >-
               Any association between a chemical and a pathway
           meaning: biolink:ChemicalToPathwayAssociation
       gene_function:
           description: >-
               Any association between a gene and molecular activity
           meaning: biolink:MacromolecularMachineToMolecularActivityAssociation
-      gene_associated_with_disease:
+      correlated_gene:
         description: >-
-          Association between a gene and a disease that is not known to affect risk
-        meaning: biolink:gene_associated_with_disease
-      gene_affects_risk_for_disease:
+          Association between a gene and a disease that has not been established to be causal
+      causal_gene:
           description: >-
-              Association between a gene and a disease that is known to affect risk
-          meaning: biolink:affects_risk_for
+              Association between a gene and a disease that is known to be causal
+          meaning: biolink:causal
 
 classes:
   Association:
     slots:
     - aggregator_knowledge_source
     - id
     - subject
@@ -84,21 +83,14 @@
     - has_evidence
     - onset_qualifier
     - sex_qualifier
     - source
     - stage_qualifier
     - pathway
     - relation
-  AssociationCount:
-    is_a: FacetValue
-    slots:
-      - id
-    slot_usage:
-      label:
-        identifier: false
   AssociationResults:
     is_a: Results
     slots: 
       - items
     slot_usage:
       items:
         range: Association
@@ -159,22 +151,51 @@
   FacetField:
     slots:
       - label
       - facet_values
     slot_usage:
       label:
         identifier: true
+  AssociationTypeMapping:
+    description: >-
+      A data class to hold the necessary information to produce association type counts for given 
+      entities with appropriate directional labels
+    slots:
+      - association_type
+      - subject_label
+      - object_label
+      - category
+      - predicate
+    slot_usage:
+      subject_label:
+        description: A label to describe the subjects of the association type as a whole for use in the UI
+      object_label:
+        description: A label to describe the objects of the association type as a whole for use in the UI
+      category:
+        description: The biolink categories to use in queries for this association type, assuming OR semantics
+        multivalued: true
+      predicate:
+        description: The biolink predicate to use in queries for this association type, assuming OR semantics
+        multivalued: true
+  AssociationCount:
+    is_a: FacetValue
+    slots:
+      - association_type
+  AssociationCountList:
+    description: Container class for a list of association counts
+    slots:
+      - items
+    slot_usage:
+      items:
+        range: AssociationCount
 slots:
   aggregator_knowledge_source:
     multivalued: true
-  associations:
-    inlined: true
-    inlined_as_list: true
-    multivalued: true
-    range: Association
+  association_type:
+    range: AssociationTypeEnum
   category:
     multivalued: true
   count:
     description: number of items a this facet value
     range: integer
   description:
     range: string
```

### Comparing `monarch_py-0.6.2/src/monarch_py/datamodels/solr.py` & `monarch_py-0.7.0/src/monarch_py/datamodels/solr.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.2/src/monarch_py/implementations/solr/solr_implementation.py` & `monarch_py-0.7.0/src/monarch_py/implementations/solr/solr_implementation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,39 @@
 import os
 from dataclasses import dataclass
-from enum import Enum
 from typing import Dict, List, Tuple
 
 from loguru import logger
 from pydantic import ValidationError
 
 from monarch_py.datamodels.model import (
     Association,
     AssociationCount,
-    AssociationLabel,
     AssociationResults,
+    AssociationTypeEnum,
     Entity,
     FacetField,
     FacetValue,
     HistoPheno,
     SearchResult,
     SearchResults,
 )
 from monarch_py.datamodels.solr import HistoPhenoKeys, SolrQuery, core
 from monarch_py.interfaces.association_interface import AssociationInterface
 from monarch_py.interfaces.entity_interface import EntityInterface
 from monarch_py.interfaces.search_interface import SearchInterface
 from monarch_py.service.solr_service import SolrService
+from monarch_py.utils.association_type_utils import (
+    AssociationTypeMappings,
+    get_association_type_mapping_by_query_string,
+    get_solr_query_fragment,
+)
 from monarch_py.utils.utils import escape
 
 
-class AssociationLabelQuery(Enum):
-    disease_phenotype = 'category:"biolink:DiseaseToPhenotypicFeatureAssociation"'
-    gene_phenotype = 'category:"biolink:GeneToPhenotypicFeatureAssociation"'
-    gene_interaction = 'category:"biolink:PairwiseGeneToGeneInteraction"'
-    gene_pathway = 'category:"biolink:GeneToPathwayAssociation"'
-    gene_expression = 'category:"biolink:GeneToExpressionSiteAssociation"'
-    gene_orthology = 'category:"biolink:GeneToGeneHomologyAssociation"'
-    chemical_pathway = 'category:"biolink:ChemicalToPathwayAssociation"'
-    gene_function = (
-        'category:"biolink:MacromolecularMachineToMolecularActivityAssociation"'
-    )
-    gene_associated_with_disease = 'category:"biolink:GeneToDiseaseAssociation" AND predicate:"biolink:gene_associated_with_condition"'
-    gene_affects_risk_for_disease = 'category:"biolink:GeneToDiseaseAssociation" AND predicate:"biolink:affects_risk_for"'
-
-
 @dataclass
 class SolrImplementation(EntityInterface, AssociationInterface, SearchInterface):
     """Implementation of Monarch Interfaces for Solr endpoint"""
 
     base_url: str = os.getenv("MONARCH_SOLR_URL", "http://localhost:8983/solr")
 
     ###############################
@@ -80,15 +69,15 @@
         subject: str = None,
         object: str = None,
         subject_closure: str = None,
         object_closure: str = None,
         entity: str = None,
         between: str = None,
         direct: bool = None,
-        association_label: AssociationLabel = None,
+        association_type: AssociationTypeEnum = None,
         offset: int = 0,
         limit: int = 20,
     ) -> AssociationResults:
         """Retrieve paginated association records, with filter options
 
         Args:
             category (str, optional): Filter to only associations matching the specified category. Defaults to None.
@@ -114,15 +103,15 @@
             subject=subject,
             object=object,
             subject_closure=subject_closure,
             object_closure=object_closure,
             entity=entity,
             between=between,
             direct=direct,
-            association_label=association_label,
+            association_type=association_type,
             offset=offset,
             limit=limit,
         )
 
         query_result = solr.query(query)
         total = query_result.response.num_found
 
@@ -148,15 +137,15 @@
         subject: str = None,
         object: str = None,
         subject_closure: str = None,
         object_closure: str = None,
         entity: str = None,
         between: str = None,
         direct: bool = None,
-        association_label: AssociationLabel = None,
+        association_type: AssociationTypeEnum = None,
         offset: int = 0,
         limit: int = 20,
     ) -> SolrQuery:
         """Populate a SolrQuery object with association filters"""
 
         query = SolrQuery(start=offset, rows=limit)
 
@@ -183,16 +172,20 @@
             query.add_filter_query(
                 f'({subject_field}:"{e1}" AND {object_field}:"{e2}") OR ({subject_field}:"{e2}" AND {object_field}:"{e1}")'
             )
         if entity:
             query.add_filter_query(
                 f'{subject_field}:"{escape(entity)}" OR {object_field}:"{escape(entity)}"'
             )
-        if association_label:
-            query.add_filter_query(AssociationLabelQuery[association_label].value)
+        if association_type:
+            query.add_filter_query(
+                get_solr_query_fragment(
+                    AssociationTypeMappings().get_mapping(association_type)
+                )
+            )
 
         return query
 
     ###############################
     # Implements: SearchInterface #
     ###############################
 
@@ -384,28 +377,63 @@
         hp = HistoPheno(
             id=subject_closure,
             items=association_counts,
         )
 
         return hp
 
-    def get_association_counts(self, entity: str) -> List[FacetValue]:
+    def get_association_counts(self, entity: str) -> List[AssociationCount]:
+        """
+        Get association counts for a given entity
+
+        This method uses chunks of solr query syntax mapped to the association type
+        Args:
+            entity:
 
-        query = self._populate_association_query(entity=entity)
-        query.facet_queries = [alq.value for alq in AssociationLabelQuery]
+        Returns:
 
+        """
+        query = self._populate_association_query(entity=entity)
+        facet_queries = []
+        subject_query = f'AND subject_closure:"{entity}"'
+        object_query = f'AND object_closure:"{entity}"'
+        # Run the same facet_queries constrained to matches against either the subject or object
+        # to know which kind of label will be needed in the UI to refer to the opposite side of the association
+        for field_query in [subject_query, object_query]:
+            for agm in AssociationTypeMappings.get_mappings():
+                association_type_query = get_solr_query_fragment(agm)
+                facet_queries.append(f"({association_type_query}) {field_query}")
+        query.facet_queries = facet_queries
         solr = SolrService(base_url=self.base_url, core=core.ASSOCIATION)
         query_result = solr.query(query)
-        facet_values: List[FacetValue] = []
+        association_counts: List[AssociationCount] = []
         for k, v in query_result.facet_counts.facet_queries.items():
             if v > 0:
-                facet_values.append(
-                    FacetValue(label=AssociationLabelQuery(k).name, count=v)
+                if k.endswith(subject_query):
+                    original_query = (
+                        k.replace(f" {subject_query}", "").lstrip("(").rstrip(")")
+                    )
+                    agm = get_association_type_mapping_by_query_string(original_query)
+                    label = agm.object_label
+                elif k.endswith(object_query):
+                    original_query = (
+                        k.replace(f" {object_query}", "").lstrip("(").rstrip(")")
+                    )
+                    agm = get_association_type_mapping_by_query_string(original_query)
+                    label = agm.subject_label
+                else:
+                    raise ValueError(
+                        f"Unexpected facet query when building association counts: {k}"
+                    )
+                association_counts.append(
+                    AssociationCount(
+                        label=label, count=v, association_type=agm.association_type
+                    )
                 )
-        return facet_values
+        return association_counts
 
     def _convert_facet_fields(self, solr_facet_fields: Dict) -> Dict[str, FacetField]:
         """
         Converts a list of raw solr facet fields from the solr response to a list of
         FacetField instances
 
         Args:
```

### Comparing `monarch_py-0.6.2/src/monarch_py/implementations/sql/sql_implementation.py` & `monarch_py-0.7.0/src/monarch_py/implementations/sql/sql_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         predicate: str = None,
         subject: str = None,
         object: str = None,
         subject_closure: str = None,
         object_closure: str = None,
         entity: str = None,
         between: str = None,
-        association_label: str = None,
+        association_type: str = None,
         offset: int = 0,
         limit: int = 20,
         update: bool = False,
     ) -> AssociationResults:
         """Retrieve paginated association records, with filter options
 
         Args:
@@ -110,15 +110,15 @@
             predicate (str, optional): Filter to only associations matching the specified predicate. Defaults to None.
             subject (str, optional): Filter to only associations matching the specified subject. Defaults to None.
             object (str, optional): Filter to only associations matching the specified object. Defaults to None.
             subject_closure (str, optional): Filter to only associations with the specified term ID as an ancestor of the subject. Defaults to None.
             object_closure (str, optional): Filter to only associations the specified term ID as an ancestor of the object. Defaults to None.
             entity (str, optional): Filter to only associations where the specified entity is the subject or the object. Defaults to None.
             between (Tuple[str, str], optional): Filter to bi-directional associations between two entities.
-            association_label (str, optional): Filter to only associations matching the specified association label. Defaults to None.
+            association_type (str, optional): Filter to only associations matching the specified association label. Defaults to None.
             offset (int, optional): Result offset, for pagination. Defaults to 0.
             limit (int, optional): Limit results to specified number. Defaults to 20.
 
         Returns:
             AssociationResults: Dataclass representing results of an association search.
         """
 
@@ -141,16 +141,16 @@
             # todo: handle error reporting / parsing, think about another way to pass this?
             b = between.split(",")
             e1 = b[0]
             e2 = b[1]
             clauses.append(
                 f"subject = '{e1}' AND object = '{e2}' OR subject = '{e2}' AND object = '{e1}'"
             )
-        if association_label:
-            clauses.append(AssociationLabelQuery[association_label].value)
+        if association_type:
+            clauses.append(AssociationLabelQuery[association_type].value)
 
         query = f"SELECT * FROM denormalized_edges "
         if clauses:
             query += "WHERE " + " AND ".join(clauses)
         if limit:
             query += f" LIMIT {limit} OFFSET {offset}"
```

### Comparing `monarch_py-0.6.2/src/monarch_py/interfaces/association_interface.py` & `monarch_py-0.7.0/src/monarch_py/interfaces/association_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,30 +14,30 @@
         predicate: str = None,
         subject: str = None,
         subject_closure: str = None,
         object: str = None,
         object_closure: str = None,
         entity: str = None,
         between: Tuple[str, str] = None,
-        association_label: str = None,
+        association_type: str = None,
         offset: int = 0,
         limit: int = 20,
     ) -> AssociationResults:
         """Retrieve paginated association records, with filter options
 
         Args:
             category (str, optional): Filter to only associations matching the specified category. Defaults to None.
             predicate (str, optional): Filter to only associations matching the specified predicate. Defaults to None.
             subject (str, optional): Filter to only associations matching the specified subject. Defaults to None.
             subject_closure (str, optional): Filter to only associations with the specified term ID as an ancestor of the subject. Defaults to None
             object (str, optional): Filter to only associations matching the specified object. Defaults to None.
             object_closure (str, optional): Filter to only associations with the specified term ID as an ancestor of the object. Defaults to None
             entity (str, optional): Filter to only associations where the specified entity is the subject or the object. Defaults to None.
             between (Tuple[str, str], optional): Filter to bi-directional associations between two entities.
-            association_label (str, optional): Filter to only associations matching the specified association label. Defaults to None.
+            association_type (str, optional): Filter to only associations matching the specified association label. Defaults to None.
             offset (int, optional): Result offset, for pagination. Defaults to 0.
             limit (int, optional): Limit results to specified number. Defaults to 20.
 
         Raises:
             NotImplementedError: Use a specific implementation (see the documentation for a list of implementations)
 
         Returns:
```

### Comparing `monarch_py-0.6.2/src/monarch_py/interfaces/entity_interface.py` & `monarch_py-0.7.0/src/monarch_py/interfaces/entity_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.2/src/monarch_py/interfaces/query_interface.py` & `monarch_py-0.7.0/src/monarch_py/interfaces/query_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.6.2/src/monarch_py/interfaces/search_interface.py` & `monarch_py-0.7.0/src/monarch_py/interfaces/search_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 from typing import List, Tuple
 
-from monarch_py.datamodels.model import AssociationLabel, FacetValue, SearchResults
+from monarch_py.datamodels.model import AssociationTypeEnum, FacetValue, SearchResults
 
 
 class SearchInterface(ABC):
     """Abstract interface for searching the Monarch KG in a Lucene way"""
 
     @abstractmethod
     def search(
@@ -58,15 +58,15 @@
         predicate: str = None,
         subject: str = None,
         subject_closure: str = None,
         object: str = None,
         object_closure: str = None,
         entity: str = None,
         between: Tuple[str, str] = None,
-        association_label: AssociationLabel = None,
+        association_type: AssociationTypeEnum = None,
     ) -> SearchResults:
         """
         Get facet counts and facet query counts for associations
         Args:
             facet_fields (List[str]): Facet fields to return counts for
             facet_queries (List[str]): Facet queries to return counts for
             category (str): Filter to only associations matching the specified category
```

### Comparing `monarch_py-0.6.2/src/monarch_py/service/solr_service.py` & `monarch_py-0.7.0/src/monarch_py/service/solr_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         response.raise_for_status()
         entity = response.json()["doc"]
         self._strip_json(entity, "_version_")
         return entity
 
     def query(self, q: SolrQuery) -> SolrQueryResult:
         url = f"{self.base_url}/{self.core.value}/select?{q.query_string()}"
-        console.log(f"Solr request: {url}")
+        logger.debug(f"Solr request: {url}")
         response = requests.get(url)
 
         data = json.loads(response.text)
         if "error" in data:
             logger.error("Solr error message: " + data["error"]["msg"])
         response.raise_for_status()
         solr_query_result = SolrQueryResult.parse_obj(data)
```

### Comparing `monarch_py-0.6.2/src/monarch_py/solr_cli.py` & `monarch_py-0.7.0/src/monarch_py/solr_cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pystow
 import typer
 
+from monarch_py.datamodels.model import AssociationCountList
 from monarch_py.utils.solr_cli_utils import (
     check_solr_permissions,
     get_solr,
     solr_status,
     start_solr,
     stop_solr,
 )
@@ -15,15 +16,15 @@
 
 ### SOLR DOCKER COMMANDS ###
 
 
 @solr_app.command("start")
 def start(update: bool = False):
     """Starts a local Solr container."""
-    check_solr_permissions(update)
+    check_solr_permissions(update=False)
     start_solr()
 
 
 @solr_app.command("stop")
 def stop():
     """Stops the local Solr container."""
     stop_solr()
@@ -32,47 +33,49 @@
 
 @solr_app.command("status")
 def status():
     solr_status()
     raise typer.Exit()
 
 
+@solr_app.command("download")
+def download():
+    get_solr(update=True)
+    raise typer.Exit()
+
+
 ### SOLR QUERY COMMANDS ###
 
 
 @solr_app.command("entity")
 def entity(
     id: str = typer.Argument(None, help="The identifier of the entity to be retrieved"),
-    update: bool = typer.Option(
-        False, "--update", "-u", help="Whether to re-download the Monarch KG"
-    ),
     fmt: str = typer.Option(
         "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
 ):
     """
     Retrieve an entity by ID
 
     Args:
         id (str): The identifier of the entity to be retrieved
 
     Optional Args:
-        update (bool): = Whether to re-download the Monarch KG. Default False
         fmt (str): The format of the output (TSV, YAML, JSON). Default JSON
         output (str): The path to the output file. Default stdout
     """
 
     if not id:
         console.print("\n[bold red]Entity ID required.[/]\n")
         raise typer.Exit(1)
 
-    data = get_solr(update)
+    data = get_solr(update=False)
     response = data.get_entity(id)
 
     if fmt == "json":
         to_json(response, output)
     elif fmt == "tsv":
         to_tsv(response, output)
     elif fmt == "yaml":
@@ -87,20 +90,17 @@
     category: str = typer.Option(None, "--category"),
     subject: str = typer.Option(None, "--subject"),
     predicate: str = typer.Option(None, "--predicate"),
     object: str = typer.Option(None, "--object"),
     entity: str = typer.Option(None, "--entity"),
     between: str = typer.Option(None, "--between"),
     direct: bool = typer.Option(False, "--direct"),
-    association_label: str = typer.Option(None, "--label"),
+    association_type: str = typer.Option(None, "--label"),
     limit: int = typer.Option(20, "--limit"),
     offset: int = typer.Option(0, "--offset"),
-    update: bool = typer.Option(
-        False, "--update", "-u", help="Whether to re-download the Monarch KG"
-    ),
     fmt: str = typer.Option(
         "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
 ):
@@ -111,27 +111,26 @@
         category (str, optional): The category of the association.
         subject (str, optional): The subject of the association.
         predicate (str, optional): The predicate of the association.
         object (str, optional): The object of the association.
         entity (str, optional): The subject or object of the association.
         between (str, optional): Two comma-separated entities to get bi-directional associations.
         direct (bool, optional): Exclude associations with the specified subject and objects as ancestors. Default False
-        association_label (str, optional): The association label of the association
+        association_type (str, optional): The association label of the association
         limit (int, optional): The number of associations to return. Default 20
         offset (int, optional): The offset of the first association to be retrieved. Default 0
-        update (bool, optional): Whether to re-download the Monarch KG. Default False
         fmt (str): The format of the output (TSV, YAML, JSON). Default JSON
         output (str): The path to the output file. Default stdout
     """
     args = locals()
     args.pop("update", None)
     args.pop("fmt", None)
     args.pop("output", None)
 
-    data = get_solr(update)
+    data = get_solr(update=False)
     response = data.get_associations(**args)
 
     if fmt == "json":
         to_json(response, output)
     elif fmt == "tsv":
         to_tsv(response, output)
     elif fmt == "yaml":
@@ -144,17 +143,14 @@
 @solr_app.command("search")
 def search(
     q: str = typer.Option(None, "--query", "-q"),
     category: str = typer.Option(None, "--category", "-c"),
     taxon: str = typer.Option(None, "--taxon", "-t"),
     limit: int = typer.Option(20, "--limit", "-l"),
     offset: int = typer.Option(0, "--offset"),
-    update: bool = typer.Option(
-        False, "--update", "-u", help="Whether to re-download the Monarch KG"
-    ),
     fmt: str = typer.Option(
         "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
 ):
@@ -166,15 +162,15 @@
         category: The category of the entity
         taxon: The taxon of the entity
         limit: The number of entities to return
         offset: The offset of the first entity to be retrieved
         fmt (str): The format of the output (TSV, YAML, JSON). Default JSON
         output (str): The path to the output file. Default stdout
     """
-    data = get_solr(update)
+    data = get_solr(update=False)
 
     response = data.search(
         q=q, category=category, taxon=taxon, limit=limit, offset=offset
     )
 
     if fmt == "json":
         to_json(response, output)
@@ -203,15 +199,15 @@
     Args:
         q: The query string to autocomplete against
         fmt: The format of the output (TSV, YAML, JSON)
         output: The path to the output file (stdout if not specified)
 
     """
 
-    data = get_solr()
+    data = get_solr(update=False)
     response = data.autocomplete(q)
 
     if fmt == "json":
         to_json(response, output)
     elif fmt == "tsv":
         to_tsv(response, output)
     elif fmt == "yaml":
@@ -220,17 +216,14 @@
         console.print(f"\n[bold red]Format '{fmt}' not supported.[/]\n")
     raise typer.Exit()
 
 
 @solr_app.command("histopheno")
 def histopheno(
     subject: str = typer.Argument(None, help="The subject of the association"),
-    update: bool = typer.Option(
-        False, "--update", "-u", help="Whether to re-download the Monarch KG"
-    ),
     fmt: str = typer.Option(
         "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
 ):
@@ -246,19 +239,59 @@
         output (str): The path to the output file. Default stdout
     """
 
     if not subject:
         console.print("\n[bold red]Subject ID required.[/]\n")
         raise typer.Exit(1)
 
-    data = get_solr(update)
+    data = get_solr(update=False)
     response = data.get_histopheno(subject)
 
     if fmt == "json":
         to_json(response, output)
     elif fmt == "tsv":
         to_tsv(response, output)
     elif fmt == "yaml":
         to_yaml(response, output)
     else:
         console.print(f"\n[bold red[Format '{fmt}' not supported.[/]\n")
     raise typer.Exit()
+
+
+@solr_app.command("association-counts")
+def association_counts(
+    entity: str = typer.Argument(None, help="The entity to get association counts for"),
+    fmt: str = typer.Option(
+        "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
+    ),
+    output: str = typer.Option(
+        None, "--output", "-o", help="The path to the output file"
+    ),
+):
+    """
+    Retrieve the association counts for a given entity
+
+    Args:
+        entity (str): The entity to get association counts for
+
+    Optional Args:
+        update (bool): Whether to re-download the Monarch KG. Default False
+        fmt (str): The format of the output (TSV, YAML, JSON). Default JSON
+        output (str): The path to the output file. Default stdout
+    """
+
+    if not entity:
+        console.print("\n[bold red]Entity ID required.[/]\n")
+        raise typer.Exit(1)
+
+    data = get_solr(update=False)
+    response = data.get_association_counts(entity)
+    counts = AssociationCountList(items=response)
+    if fmt == "json":
+        to_json(counts, output)
+    elif fmt == "tsv":
+        to_tsv(counts, output)
+    elif fmt == "yaml":
+        to_yaml(counts, output)
+    else:
+        console.print(f"\n[bold red[Format '{fmt}' not supported.[/]\n")
+    raise typer.Exit()
```

### Comparing `monarch_py-0.6.2/src/monarch_py/sql_cli.py` & `monarch_py-0.7.0/src/monarch_py/sql_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 def associations(
     category: str = typer.Option(None, "--category"),
     subject: str = typer.Option(None, "--subject"),
     predicate: str = typer.Option(None, "--predicate"),
     object: str = typer.Option(None, "--object"),
     entity: str = typer.Option(None, "--entity"),
     between: str = typer.Option(None, "--between"),
-    association_label: str = typer.Option(None, "--label"),
+    association_type: str = typer.Option(None, "--label"),
     limit: int = typer.Option(20, "--limit"),
     offset: int = typer.Option(0, "--offset"),
     update: bool = typer.Option(False, "--update"),
     fmt: str = typer.Option(
         "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
     ),
     output: str = typer.Option(
@@ -75,15 +75,15 @@
     Args:
         category (str, optional): The category of the association.
         subject (str, optional): The subject of the association.
         predicate (str, optional): The predicate of the association.
         object (str, optional): The object of the association.
         entity (str, optional): The subject or object of the association.
         between (str, optional): Two comma-separated entities to get bi-directional associations.
-        association_label (str, optional): The label of the association.
+        association_type (str, optional): The label of the association.
         limit (int, optional): The number of associations to return. Default 20
         offset (int, optional): The offset of the first association to be retrieved. Default 0
         update (bool, optional): Whether to re-download the Monarch KG. Default False
         fmt (str): The format of the output (TSV, YAML, JSON). Default JSON
         output (str): The path to the output file. Default stdout
     """
     args = locals()
```

### Comparing `monarch_py-0.6.2/src/monarch_py/utils/solr_cli_utils.py` & `monarch_py-0.7.0/src/monarch_py/utils/solr_cli_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 import os
+import shutil
 import sys
 import time
 
 import docker
 import pystow
 
 from monarch_py.implementations.solr.solr_implementation import SolrImplementation
 from monarch_py.utils.utils import SOLR_DATA_URL, console
 
 monarchstow = pystow.module("monarch")
 
 
 def check_solr_permissions(update: bool = False) -> None:
     """Checks that the solr data directory has the correct permissions."""
+    data_path = monarchstow.base / "solr" / "data"
+    # When untarred solr won't necessarily use the same file names for index segments etc
+    # so the untarred path needs to be removed before updating
+    if update:
+        shutil.rmtree(data_path)
     monarchstow.ensure_untar(url=SOLR_DATA_URL, force=update)
     if sys.platform in ["linux", "linux2", "darwin"]:
-        stat_info = os.stat(monarchstow.base / "solr" / "data")
+        stat_info = os.stat(data_path)
         if stat_info.st_gid != 8983:
             console.print(
                 f"""
 Solr container requires write access to {monarchstow.base}.
 Please run the following command to set permissions:
     [grey84 on black]sudo chgrp -R 8983 {monarchstow.base}[/]
     [grey84 on black]sudo chmod -R g+w {monarchstow.base}[/]
@@ -33,15 +39,16 @@
         console.print("\nChecking for Solr container...")
     c = dc.containers.list(all=True, filters={"name": "monarch_solr"})
     return None if not c else c[0]
 
 
 def get_solr(update: bool = False):
     """Checks for Solr data and container, and returns a SolrImplementation."""
-    check_solr_permissions(update)
+    if update:
+        check_solr_permissions(update)
     if check_for_solr(dc=docker.from_env(), quiet=True):
         return SolrImplementation()
     else:
         console.print(
             "\nNo Solr container found!\nStart a Solr container with [bold]monarch solr start[/]."
         )
         sys.exit(1)
@@ -76,27 +83,27 @@
                 f"Error running existing container {c.name} ({c.status}) - {e}"
             )
             raise e
 
 
 def stop_solr():
     """Stops the local Solr container."""
-    c = check_for_solr(quiet=True)
+    c = check_for_solr(dc=docker.from_env(), quiet=True)
     if c:
         try:
             console.print(f"Stopping {c.name}...")
             c.stop()
             c.remove()
         except Exception as e:
             console.print(f"Error stopping container {c.name} ({c.status}) - {e}")
             raise e
 
 
 def solr_status():
-    c = check_for_solr()
+    c = check_for_solr(dc=docker.from_env())
     if not c:
         console.print(
             """
 No monarch_solr container found. 
 
 Download the Monarch Solr KG and start a local solr instance:
     [grey84 on black]monarch solr start[/]
```

### Comparing `monarch_py-0.6.2/src/monarch_py/utils/utils.py` & `monarch_py-0.7.0/src/monarch_py/utils/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 import sys
 
 import yaml
 from rich import print_json
 from rich.console import Console
 from rich.table import Table
 
-from monarch_py.datamodels.model import ConfiguredBaseModel, Entity, HistoPheno, Results
+from monarch_py.datamodels.model import (
+    AssociationCountList,
+    ConfiguredBaseModel,
+    Entity,
+    HistoPheno,
+    Results,
+)
 
 SOLR_DATA_URL = "https://data.monarchinitiative.org/monarch-kg-dev/latest/solr.tar.gz"
 SQL_DATA_URL = (
     "https://data.monarchinitiative.org/monarch-kg-dev/latest/monarch-kg.db.gz"
 )
 
 
@@ -38,17 +44,15 @@
     """Converts a sqlite3 row to a dictionary."""
     fields = [column[0] for column in cursor.description]
     return {key: value for key, value in zip(fields, row)}
 
 
 ### Output conversion methods ###
 
-FMT_INPUR_ERROR_MSG = (
-    "Text conversion method only accepts Entity, HistoPheno, or Results objects."
-)
+FMT_INPUT_ERROR_MSG = "Text conversion method only accepts Entity, HistoPheno, AssociationCountList, or Results objects."
 
 
 def to_json(obj: ConfiguredBaseModel, file: str):
     """Converts a pydantic model to a JSON string."""
     if file:
         with open(file, "w") as f:
             f.write(obj.json(indent=4))
@@ -60,19 +64,23 @@
 def to_tsv(obj: ConfiguredBaseModel, file: str) -> str:
     """Converts a pydantic model to a TSV string."""
 
     # Extract headers and rows from object
     if isinstance(obj, Entity):
         headers = obj.dict().keys()
         rows = [list(obj.dict().values())]
-    elif isinstance(obj, Results) or isinstance(obj, HistoPheno):
+    elif (
+        isinstance(obj, Results)
+        or isinstance(obj, HistoPheno)
+        or isinstance(obj, AssociationCountList)
+    ):
         headers = obj.items[0].dict().keys()
         rows = [list(item.dict().values()) for item in obj.items]
     else:
-        raise TypeError(FMT_INPUR_ERROR_MSG)
+        raise TypeError(FMT_INPUT_ERROR_MSG)
 
     # console.print(f"\n{obj.__class__.__name__}\n")
     # console.print(f"Headers ({type(headers)}): {headers}\n")
     # console.print(f"Rows ({type(rows)}):")
     # for row in rows: console.print(row)
 
     if file:
@@ -133,17 +141,21 @@
 def to_yaml(obj: ConfiguredBaseModel, file: str):
     """Converts a pydantic model to a YAML string."""
 
     fh = open(file, "w") if file else sys.stdout
 
     if isinstance(obj, Entity):
         yaml.dump(obj.dict(), fh, indent=4)
-    elif isinstance(obj, Results) or isinstance(obj, HistoPheno):
+    elif (
+        isinstance(obj, Results)
+        or isinstance(obj, HistoPheno)
+        or isinstance(obj, AssociationCountList)
+    ):
         yaml.dump([item.dict() for item in obj.items], fh, indent=4)
     else:
-        raise TypeError(FMT_INPUR_ERROR_MSG)
+        raise TypeError(FMT_INPUT_ERROR_MSG)
 
     if file:
         console.print(f"\nOutput written to {file}\n")
         fh.close()
 
     return
```

### Comparing `monarch_py-0.6.2/PKG-INFO` & `monarch_py-0.7.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monarch-py
-Version: 0.6.2
+Version: 0.7.0
 Summary: Monarch Initiative data access library
 Author: Kevin Schaper
 Author-email: kevin@tislab.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

