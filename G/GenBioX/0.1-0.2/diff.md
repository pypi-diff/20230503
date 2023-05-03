# Comparing `tmp/GenBioX-0.1.tar.gz` & `tmp/GenBioX-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GenBioX-0.1.tar", last modified: Wed May  3 06:18:27 2023, max compression
+gzip compressed data, was "GenBioX-0.2.tar", last modified: Wed May  3 09:53:22 2023, max compression
```

## Comparing `GenBioX-0.1.tar` & `GenBioX-0.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-03 06:18:27.432120 GenBioX-0.1/
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-03 06:18:27.417194 GenBioX-0.1/GenBioX/
--rw-r--r--   0 li         (501) staff       (20)        0 2023-03-12 06:16:05.000000 GenBioX-0.1/GenBioX/__init__.py
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-03 06:18:27.419870 GenBioX-0.1/GenBioX/alignment/
--rw-r--r--   0 li         (501) staff       (20)      247 2023-05-02 09:24:07.000000 GenBioX-0.1/GenBioX/alignment/__init__.py
--rw-r--r--   0 li         (501) staff       (20)      803 2023-03-29 11:45:13.000000 GenBioX-0.1/GenBioX/alignment/align.py
--rw-r--r--   0 li         (501) staff       (20)      720 2023-04-28 11:19:37.000000 GenBioX-0.1/GenBioX/alignment/evaluate_alignment_quality.py
--rw-r--r--   0 li         (501) staff       (20)     1316 2023-04-28 11:13:12.000000 GenBioX-0.1/GenBioX/alignment/extract_conserved_regions.py
--rw-r--r--   0 li         (501) staff       (20)      810 2023-04-28 11:09:16.000000 GenBioX-0.1/GenBioX/alignment/merge_alignments.py
--rw-r--r--   0 li         (501) staff       (20)      740 2023-04-28 11:39:45.000000 GenBioX-0.1/GenBioX/alignment/read_alignment.py
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-03 06:18:27.421925 GenBioX-0.1/GenBioX/annotation/
--rw-r--r--   0 li         (501) staff       (20)      155 2023-05-02 09:26:59.000000 GenBioX-0.1/GenBioX/annotation/__init__.py
--rw-r--r--   0 li         (501) staff       (20)     2719 2023-03-13 06:47:14.000000 GenBioX-0.1/GenBioX/annotation/annotation.py
--rw-r--r--   0 li         (501) staff       (20)        0 2023-03-13 05:42:34.000000 GenBioX-0.1/GenBioX/annotation/ap_qualityCheck.py
--rw-r--r--   0 li         (501) staff       (20)     1270 2023-04-28 11:23:02.000000 GenBioX-0.1/GenBioX/annotation/extract_annotations.py
--rw-r--r--   0 li         (501) staff       (20)      772 2023-04-28 11:23:46.000000 GenBioX-0.1/GenBioX/annotation/filter_annotations.py
--rw-r--r--   0 li         (501) staff       (20)      670 2023-04-28 11:24:17.000000 GenBioX-0.1/GenBioX/annotation/search_annotations.py
--rw-r--r--   0 li         (501) staff       (20)      577 2023-03-13 07:19:41.000000 GenBioX-0.1/GenBioX/annotation/test_annotation.py
--rw-r--r--   0 li         (501) staff       (20)      914 2023-03-13 06:38:01.000000 GenBioX-0.1/GenBioX/annotation/test_annotation_processing.py
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-03 06:18:27.423192 GenBioX-0.1/GenBioX/comparative_genomics/
--rw-r--r--   0 li         (501) staff       (20)      226 2023-05-02 09:35:31.000000 GenBioX-0.1/GenBioX/comparative_genomics/__init__.py
--rw-r--r--   0 li         (501) staff       (20)      627 2023-04-28 12:27:36.000000 GenBioX-0.1/GenBioX/comparative_genomics/compare_genome_size.py
--rw-r--r--   0 li         (501) staff       (20)     1003 2023-04-28 12:29:13.000000 GenBioX-0.1/GenBioX/comparative_genomics/identify_conserved_regions.py
--rw-r--r--   0 li         (501) staff       (20)     1091 2023-04-28 12:33:31.000000 GenBioX-0.1/GenBioX/comparative_genomics/pairwise_identity.py
--rw-r--r--   0 li         (501) staff       (20)      865 2023-05-02 09:34:26.000000 GenBioX-0.1/GenBioX/comparative_genomics/phylogenetic_distance.py
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-03 06:18:27.427236 GenBioX-0.1/GenBioX/data_preprocessing/
--rw-r--r--   0 li         (501) staff       (20)      498 2023-05-02 09:16:54.000000 GenBioX-0.1/GenBioX/data_preprocessing/__init__.py
--rw-r--r--   0 li         (501) staff       (20)     1269 2023-03-21 11:47:30.000000 GenBioX-0.1/GenBioX/data_preprocessing/extract_annotation.py
--rw-r--r--   0 li         (501) staff       (20)      994 2023-03-12 11:10:50.000000 GenBioX-0.1/GenBioX/data_preprocessing/fasta_quality_check.py
--rw-r--r--   0 li         (501) staff       (20)     1670 2023-03-15 07:48:07.000000 GenBioX-0.1/GenBioX/data_preprocessing/fetch_seq.py
--rw-r--r--   0 li         (501) staff       (20)      735 2023-03-21 12:36:47.000000 GenBioX-0.1/GenBioX/data_preprocessing/filter_contaminants.py
--rw-r--r--   0 li         (501) staff       (20)      819 2023-05-02 09:10:07.000000 GenBioX-0.1/GenBioX/data_preprocessing/filter_low_quality_read.py
--rw-r--r--   0 li         (501) staff       (20)      696 2023-05-02 09:07:31.000000 GenBioX-0.1/GenBioX/data_preprocessing/quality_score.py
--rw-r--r--   0 li         (501) staff       (20)      719 2023-05-01 09:51:28.000000 GenBioX-0.1/GenBioX/data_preprocessing/read_fasta.py
--rw-r--r--   0 li         (501) staff       (20)      516 2023-03-21 12:32:15.000000 GenBioX-0.1/GenBioX/data_preprocessing/remove_duplicates.py
--rw-r--r--   0 li         (501) staff       (20)      492 2023-03-12 11:43:35.000000 GenBioX-0.1/GenBioX/data_preprocessing/test2.py
--rw-r--r--   0 li         (501) staff       (20)      202 2023-03-15 07:46:06.000000 GenBioX-0.1/GenBioX/data_preprocessing/test_fetch_seq.py
--rw-r--r--   0 li         (501) staff       (20)      301 2023-03-15 07:15:50.000000 GenBioX-0.1/GenBioX/data_preprocessing/test_read_fasta.py
--rw-r--r--   0 li         (501) staff       (20)      845 2023-03-21 12:31:53.000000 GenBioX-0.1/GenBioX/data_preprocessing/trim_adapters.py
--rw-r--r--   0 li         (501) staff       (20)      466 2023-03-12 10:13:01.000000 GenBioX-0.1/GenBioX/data_preprocessing/vcf.py
--rw-r--r--   0 li         (501) staff       (20)     1725 2023-03-21 12:38:00.000000 GenBioX-0.1/GenBioX/data_preprocessing/visualise_quality_metrics.py
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-03 06:18:27.428611 GenBioX-0.1/GenBioX/gene_expression/
--rw-r--r--   0 li         (501) staff       (20)      306 2023-05-02 09:33:24.000000 GenBioX-0.1/GenBioX/gene_expression/__init__.py
--rw-r--r--   0 li         (501) staff       (20)     2381 2023-04-28 12:15:59.000000 GenBioX-0.1/GenBioX/gene_expression/differential_gene_expression_analysis.py
--rw-r--r--   0 li         (501) staff       (20)      857 2023-04-28 12:19:43.000000 GenBioX-0.1/GenBioX/gene_expression/gene_expression_correlation.py
--rw-r--r--   0 li         (501) staff       (20)      968 2023-04-28 12:13:21.000000 GenBioX-0.1/GenBioX/gene_expression/gene_expression_normalization.py
--rw-r--r--   0 li         (501) staff       (20)      834 2023-04-28 12:18:09.000000 GenBioX-0.1/GenBioX/gene_expression/gene_expression_quantification.py
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-03 06:18:27.429928 GenBioX-0.1/GenBioX/statistical_analysis/
--rw-r--r--   0 li         (501) staff       (20)      189 2023-05-02 09:20:21.000000 GenBioX-0.1/GenBioX/statistical_analysis/__init__.py
--rw-r--r--   0 li         (501) staff       (20)      313 2023-03-29 10:45:48.000000 GenBioX-0.1/GenBioX/statistical_analysis/calculate_gc_content.py
--rw-r--r--   0 li         (501) staff       (20)      638 2023-03-29 11:26:06.000000 GenBioX-0.1/GenBioX/statistical_analysis/count_nucleotides.py
--rw-r--r--   0 li         (501) staff       (20)      606 2023-03-29 11:13:34.000000 GenBioX-0.1/GenBioX/statistical_analysis/reverse_complement.py
--rw-r--r--   0 li         (501) staff       (20)      911 2023-03-29 11:07:19.000000 GenBioX-0.1/GenBioX/statistical_analysis/translate.py
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-03 06:18:27.431438 GenBioX-0.1/GenBioX/variant_analysis/
--rw-r--r--   0 li         (501) staff       (20)      275 2023-05-02 09:30:22.000000 GenBioX-0.1/GenBioX/variant_analysis/__init__.py
--rw-r--r--   0 li         (501) staff       (20)      993 2023-05-02 09:29:28.000000 GenBioX-0.1/GenBioX/variant_analysis/phenotype_prediction.py
--rw-r--r--   0 li         (501) staff       (20)     1041 2023-04-28 11:57:24.000000 GenBioX-0.1/GenBioX/variant_analysis/splice_site_prediction.py
--rw-r--r--   0 li         (501) staff       (20)      673 2023-04-28 11:53:06.000000 GenBioX-0.1/GenBioX/variant_analysis/variant_annotation.py
--rw-r--r--   0 li         (501) staff       (20)      437 2023-04-28 11:51:00.000000 GenBioX-0.1/GenBioX/variant_analysis/variant_calling.py
--rw-r--r--   0 li         (501) staff       (20)      608 2023-04-28 11:54:44.000000 GenBioX-0.1/GenBioX/variant_analysis/variant_effect_prediction.py
-drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-03 06:18:27.417770 GenBioX-0.1/GenBioX.egg-info/
--rw-r--r--   0 li         (501) staff       (20)      668 2023-05-03 06:18:27.000000 GenBioX-0.1/GenBioX.egg-info/PKG-INFO
--rw-r--r--   0 li         (501) staff       (20)     2443 2023-05-03 06:18:27.000000 GenBioX-0.1/GenBioX.egg-info/SOURCES.txt
--rw-r--r--   0 li         (501) staff       (20)        1 2023-05-03 06:18:27.000000 GenBioX-0.1/GenBioX.egg-info/dependency_links.txt
--rw-r--r--   0 li         (501) staff       (20)       64 2023-05-03 06:18:27.000000 GenBioX-0.1/GenBioX.egg-info/requires.txt
--rw-r--r--   0 li         (501) staff       (20)        8 2023-05-03 06:18:27.000000 GenBioX-0.1/GenBioX.egg-info/top_level.txt
--rw-r--r--   0 li         (501) staff       (20)      668 2023-05-03 06:18:27.431791 GenBioX-0.1/PKG-INFO
--rw-r--r--   0 li         (501) staff       (20)       38 2023-05-03 06:18:27.432170 GenBioX-0.1/setup.cfg
--rw-r--r--   0 li         (501) staff       (20)      923 2023-05-01 09:10:01.000000 GenBioX-0.1/setup.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-03 09:53:22.640351 GenBioX-0.2/
+drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-03 09:53:22.625751 GenBioX-0.2/GenBioX/
+-rw-r--r--   0 li         (501) staff       (20)        0 2023-03-12 06:16:05.000000 GenBioX-0.2/GenBioX/__init__.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-03 09:53:22.627986 GenBioX-0.2/GenBioX/alignment/
+-rw-r--r--   0 li         (501) staff       (20)      247 2023-05-02 09:24:07.000000 GenBioX-0.2/GenBioX/alignment/__init__.py
+-rw-r--r--   0 li         (501) staff       (20)      803 2023-03-29 11:45:13.000000 GenBioX-0.2/GenBioX/alignment/align.py
+-rw-r--r--   0 li         (501) staff       (20)      720 2023-04-28 11:19:37.000000 GenBioX-0.2/GenBioX/alignment/evaluate_alignment_quality.py
+-rw-r--r--   0 li         (501) staff       (20)     1316 2023-04-28 11:13:12.000000 GenBioX-0.2/GenBioX/alignment/extract_conserved_regions.py
+-rw-r--r--   0 li         (501) staff       (20)      810 2023-04-28 11:09:16.000000 GenBioX-0.2/GenBioX/alignment/merge_alignments.py
+-rw-r--r--   0 li         (501) staff       (20)      740 2023-04-28 11:39:45.000000 GenBioX-0.2/GenBioX/alignment/read_alignment.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-03 09:53:22.630076 GenBioX-0.2/GenBioX/annotation/
+-rw-r--r--   0 li         (501) staff       (20)      155 2023-05-02 09:26:59.000000 GenBioX-0.2/GenBioX/annotation/__init__.py
+-rw-r--r--   0 li         (501) staff       (20)     2719 2023-03-13 06:47:14.000000 GenBioX-0.2/GenBioX/annotation/annotation.py
+-rw-r--r--   0 li         (501) staff       (20)        0 2023-03-13 05:42:34.000000 GenBioX-0.2/GenBioX/annotation/ap_qualityCheck.py
+-rw-r--r--   0 li         (501) staff       (20)     1270 2023-04-28 11:23:02.000000 GenBioX-0.2/GenBioX/annotation/extract_annotations.py
+-rw-r--r--   0 li         (501) staff       (20)      772 2023-04-28 11:23:46.000000 GenBioX-0.2/GenBioX/annotation/filter_annotations.py
+-rw-r--r--   0 li         (501) staff       (20)      670 2023-04-28 11:24:17.000000 GenBioX-0.2/GenBioX/annotation/search_annotations.py
+-rw-r--r--   0 li         (501) staff       (20)      577 2023-03-13 07:19:41.000000 GenBioX-0.2/GenBioX/annotation/test_annotation.py
+-rw-r--r--   0 li         (501) staff       (20)      914 2023-03-13 06:38:01.000000 GenBioX-0.2/GenBioX/annotation/test_annotation_processing.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-03 09:53:22.631347 GenBioX-0.2/GenBioX/comparative_genomics/
+-rw-r--r--   0 li         (501) staff       (20)      226 2023-05-02 09:35:31.000000 GenBioX-0.2/GenBioX/comparative_genomics/__init__.py
+-rw-r--r--   0 li         (501) staff       (20)      627 2023-04-28 12:27:36.000000 GenBioX-0.2/GenBioX/comparative_genomics/compare_genome_size.py
+-rw-r--r--   0 li         (501) staff       (20)     1003 2023-04-28 12:29:13.000000 GenBioX-0.2/GenBioX/comparative_genomics/identify_conserved_regions.py
+-rw-r--r--   0 li         (501) staff       (20)     1091 2023-04-28 12:33:31.000000 GenBioX-0.2/GenBioX/comparative_genomics/pairwise_identity.py
+-rw-r--r--   0 li         (501) staff       (20)      865 2023-05-02 09:34:26.000000 GenBioX-0.2/GenBioX/comparative_genomics/phylogenetic_distance.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-03 09:53:22.635540 GenBioX-0.2/GenBioX/data_preprocessing/
+-rw-r--r--   0 li         (501) staff       (20)      498 2023-05-02 09:16:54.000000 GenBioX-0.2/GenBioX/data_preprocessing/__init__.py
+-rw-r--r--   0 li         (501) staff       (20)     1269 2023-03-21 11:47:30.000000 GenBioX-0.2/GenBioX/data_preprocessing/extract_annotation.py
+-rw-r--r--   0 li         (501) staff       (20)      994 2023-03-12 11:10:50.000000 GenBioX-0.2/GenBioX/data_preprocessing/fasta_quality_check.py
+-rw-r--r--   0 li         (501) staff       (20)     1670 2023-03-15 07:48:07.000000 GenBioX-0.2/GenBioX/data_preprocessing/fetch_seq.py
+-rw-r--r--   0 li         (501) staff       (20)      735 2023-03-21 12:36:47.000000 GenBioX-0.2/GenBioX/data_preprocessing/filter_contaminants.py
+-rw-r--r--   0 li         (501) staff       (20)      819 2023-05-02 09:10:07.000000 GenBioX-0.2/GenBioX/data_preprocessing/filter_low_quality_read.py
+-rw-r--r--   0 li         (501) staff       (20)      696 2023-05-02 09:07:31.000000 GenBioX-0.2/GenBioX/data_preprocessing/quality_score.py
+-rw-r--r--   0 li         (501) staff       (20)      719 2023-05-01 09:51:28.000000 GenBioX-0.2/GenBioX/data_preprocessing/read_fasta.py
+-rw-r--r--   0 li         (501) staff       (20)      516 2023-03-21 12:32:15.000000 GenBioX-0.2/GenBioX/data_preprocessing/remove_duplicates.py
+-rw-r--r--   0 li         (501) staff       (20)      492 2023-03-12 11:43:35.000000 GenBioX-0.2/GenBioX/data_preprocessing/test2.py
+-rw-r--r--   0 li         (501) staff       (20)      202 2023-03-15 07:46:06.000000 GenBioX-0.2/GenBioX/data_preprocessing/test_fetch_seq.py
+-rw-r--r--   0 li         (501) staff       (20)      301 2023-03-15 07:15:50.000000 GenBioX-0.2/GenBioX/data_preprocessing/test_read_fasta.py
+-rw-r--r--   0 li         (501) staff       (20)      845 2023-03-21 12:31:53.000000 GenBioX-0.2/GenBioX/data_preprocessing/trim_adapters.py
+-rw-r--r--   0 li         (501) staff       (20)      466 2023-03-12 10:13:01.000000 GenBioX-0.2/GenBioX/data_preprocessing/vcf.py
+-rw-r--r--   0 li         (501) staff       (20)     1725 2023-03-21 12:38:00.000000 GenBioX-0.2/GenBioX/data_preprocessing/visualise_quality_metrics.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-03 09:53:22.636933 GenBioX-0.2/GenBioX/gene_expression/
+-rw-r--r--   0 li         (501) staff       (20)      306 2023-05-02 09:33:24.000000 GenBioX-0.2/GenBioX/gene_expression/__init__.py
+-rw-r--r--   0 li         (501) staff       (20)     2381 2023-04-28 12:15:59.000000 GenBioX-0.2/GenBioX/gene_expression/differential_gene_expression_analysis.py
+-rw-r--r--   0 li         (501) staff       (20)      857 2023-04-28 12:19:43.000000 GenBioX-0.2/GenBioX/gene_expression/gene_expression_correlation.py
+-rw-r--r--   0 li         (501) staff       (20)      968 2023-04-28 12:13:21.000000 GenBioX-0.2/GenBioX/gene_expression/gene_expression_normalization.py
+-rw-r--r--   0 li         (501) staff       (20)      834 2023-04-28 12:18:09.000000 GenBioX-0.2/GenBioX/gene_expression/gene_expression_quantification.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-03 09:53:22.638248 GenBioX-0.2/GenBioX/statistical_analysis/
+-rw-r--r--   0 li         (501) staff       (20)      189 2023-05-02 09:20:21.000000 GenBioX-0.2/GenBioX/statistical_analysis/__init__.py
+-rw-r--r--   0 li         (501) staff       (20)      313 2023-03-29 10:45:48.000000 GenBioX-0.2/GenBioX/statistical_analysis/calculate_gc_content.py
+-rw-r--r--   0 li         (501) staff       (20)      638 2023-03-29 11:26:06.000000 GenBioX-0.2/GenBioX/statistical_analysis/count_nucleotides.py
+-rw-r--r--   0 li         (501) staff       (20)      606 2023-03-29 11:13:34.000000 GenBioX-0.2/GenBioX/statistical_analysis/reverse_complement.py
+-rw-r--r--   0 li         (501) staff       (20)      911 2023-03-29 11:07:19.000000 GenBioX-0.2/GenBioX/statistical_analysis/translate.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-03 09:53:22.639743 GenBioX-0.2/GenBioX/variant_analysis/
+-rw-r--r--   0 li         (501) staff       (20)      275 2023-05-02 09:30:22.000000 GenBioX-0.2/GenBioX/variant_analysis/__init__.py
+-rw-r--r--   0 li         (501) staff       (20)      993 2023-05-02 09:29:28.000000 GenBioX-0.2/GenBioX/variant_analysis/phenotype_prediction.py
+-rw-r--r--   0 li         (501) staff       (20)     1041 2023-04-28 11:57:24.000000 GenBioX-0.2/GenBioX/variant_analysis/splice_site_prediction.py
+-rw-r--r--   0 li         (501) staff       (20)      673 2023-04-28 11:53:06.000000 GenBioX-0.2/GenBioX/variant_analysis/variant_annotation.py
+-rw-r--r--   0 li         (501) staff       (20)      437 2023-04-28 11:51:00.000000 GenBioX-0.2/GenBioX/variant_analysis/variant_calling.py
+-rw-r--r--   0 li         (501) staff       (20)      608 2023-04-28 11:54:44.000000 GenBioX-0.2/GenBioX/variant_analysis/variant_effect_prediction.py
+drwxr-xr-x   0 li         (501) staff       (20)        0 2023-05-03 09:53:22.626365 GenBioX-0.2/GenBioX.egg-info/
+-rw-r--r--   0 li         (501) staff       (20)      729 2023-05-03 09:53:22.000000 GenBioX-0.2/GenBioX.egg-info/PKG-INFO
+-rw-r--r--   0 li         (501) staff       (20)     2443 2023-05-03 09:53:22.000000 GenBioX-0.2/GenBioX.egg-info/SOURCES.txt
+-rw-r--r--   0 li         (501) staff       (20)        1 2023-05-03 09:53:22.000000 GenBioX-0.2/GenBioX.egg-info/dependency_links.txt
+-rw-r--r--   0 li         (501) staff       (20)       64 2023-05-03 09:53:22.000000 GenBioX-0.2/GenBioX.egg-info/requires.txt
+-rw-r--r--   0 li         (501) staff       (20)        8 2023-05-03 09:53:22.000000 GenBioX-0.2/GenBioX.egg-info/top_level.txt
+-rw-r--r--   0 li         (501) staff       (20)      729 2023-05-03 09:53:22.640075 GenBioX-0.2/PKG-INFO
+-rw-r--r--   0 li         (501) staff       (20)       38 2023-05-03 09:53:22.640404 GenBioX-0.2/setup.cfg
+-rw-r--r--   0 li         (501) staff       (20)     1012 2023-05-03 09:52:59.000000 GenBioX-0.2/setup.py
```

### Comparing `GenBioX-0.1/GenBioX/alignment/align.py` & `GenBioX-0.2/GenBioX/alignment/align.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/alignment/evaluate_alignment_quality.py` & `GenBioX-0.2/GenBioX/alignment/evaluate_alignment_quality.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/alignment/extract_conserved_regions.py` & `GenBioX-0.2/GenBioX/alignment/extract_conserved_regions.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/alignment/merge_alignments.py` & `GenBioX-0.2/GenBioX/alignment/merge_alignments.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/alignment/read_alignment.py` & `GenBioX-0.2/GenBioX/alignment/read_alignment.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/annotation/annotation.py` & `GenBioX-0.2/GenBioX/annotation/annotation.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/annotation/extract_annotations.py` & `GenBioX-0.2/GenBioX/annotation/extract_annotations.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/annotation/filter_annotations.py` & `GenBioX-0.2/GenBioX/annotation/filter_annotations.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/annotation/search_annotations.py` & `GenBioX-0.2/GenBioX/annotation/search_annotations.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/annotation/test_annotation.py` & `GenBioX-0.2/GenBioX/annotation/test_annotation.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/annotation/test_annotation_processing.py` & `GenBioX-0.2/GenBioX/annotation/test_annotation_processing.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/comparative_genomics/compare_genome_size.py` & `GenBioX-0.2/GenBioX/comparative_genomics/compare_genome_size.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/comparative_genomics/identify_conserved_regions.py` & `GenBioX-0.2/GenBioX/comparative_genomics/identify_conserved_regions.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/comparative_genomics/pairwise_identity.py` & `GenBioX-0.2/GenBioX/comparative_genomics/pairwise_identity.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/comparative_genomics/phylogenetic_distance.py` & `GenBioX-0.2/GenBioX/comparative_genomics/phylogenetic_distance.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/data_preprocessing/extract_annotation.py` & `GenBioX-0.2/GenBioX/data_preprocessing/extract_annotation.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/data_preprocessing/fasta_quality_check.py` & `GenBioX-0.2/GenBioX/data_preprocessing/fasta_quality_check.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/data_preprocessing/fetch_seq.py` & `GenBioX-0.2/GenBioX/data_preprocessing/fetch_seq.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/data_preprocessing/filter_contaminants.py` & `GenBioX-0.2/GenBioX/data_preprocessing/filter_contaminants.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/data_preprocessing/filter_low_quality_read.py` & `GenBioX-0.2/GenBioX/data_preprocessing/filter_low_quality_read.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/data_preprocessing/quality_score.py` & `GenBioX-0.2/GenBioX/data_preprocessing/quality_score.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/data_preprocessing/read_fasta.py` & `GenBioX-0.2/GenBioX/data_preprocessing/read_fasta.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/data_preprocessing/remove_duplicates.py` & `GenBioX-0.2/GenBioX/data_preprocessing/remove_duplicates.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/data_preprocessing/trim_adapters.py` & `GenBioX-0.2/GenBioX/data_preprocessing/trim_adapters.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/data_preprocessing/visualise_quality_metrics.py` & `GenBioX-0.2/GenBioX/data_preprocessing/visualise_quality_metrics.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/gene_expression/differential_gene_expression_analysis.py` & `GenBioX-0.2/GenBioX/gene_expression/differential_gene_expression_analysis.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/gene_expression/gene_expression_correlation.py` & `GenBioX-0.2/GenBioX/gene_expression/gene_expression_correlation.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/gene_expression/gene_expression_normalization.py` & `GenBioX-0.2/GenBioX/gene_expression/gene_expression_normalization.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/gene_expression/gene_expression_quantification.py` & `GenBioX-0.2/GenBioX/gene_expression/gene_expression_quantification.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/statistical_analysis/count_nucleotides.py` & `GenBioX-0.2/GenBioX/statistical_analysis/count_nucleotides.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/statistical_analysis/reverse_complement.py` & `GenBioX-0.2/GenBioX/statistical_analysis/reverse_complement.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/statistical_analysis/translate.py` & `GenBioX-0.2/GenBioX/statistical_analysis/translate.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/variant_analysis/phenotype_prediction.py` & `GenBioX-0.2/GenBioX/variant_analysis/phenotype_prediction.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/variant_analysis/splice_site_prediction.py` & `GenBioX-0.2/GenBioX/variant_analysis/splice_site_prediction.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/variant_analysis/variant_annotation.py` & `GenBioX-0.2/GenBioX/variant_analysis/variant_annotation.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX/variant_analysis/variant_effect_prediction.py` & `GenBioX-0.2/GenBioX/variant_analysis/variant_effect_prediction.py`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/GenBioX.egg-info/SOURCES.txt` & `GenBioX-0.2/GenBioX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GenBioX-0.1/setup.py` & `GenBioX-0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='GenBioX',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     license='MIT',
     description='A package for Genome Analysis',
+     long_description='''For documentation, please visit http://genbiox.readthedocs.io/''',
     install_requires=[
         'pandas>=1.3.0',
         'numpy>=1.21.1',
         'Biopython>=1.79',
         'scikit-allel>=1.3.2'
     ],
-    url='https://github.com/SayaGarud/ResistomeX.git',
+    url='https://github.com/SayaGarud/GenBioX.git',
     author='Sayali Garud',
     author_email='sayaligrud@gmail.com',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

