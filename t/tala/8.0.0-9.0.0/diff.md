# Comparing `tmp/tala-8.0.0-py3-none-any.whl.zip` & `tmp/tala-9.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,240 +1,251 @@
-Zip file size: 206773 bytes, number of entries: 238
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 bin/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 integration_tests/__init__.py
--rw-r--r--  2.0 unx    31685 b- defN 20-Sep-09 09:08 integration_tests/test_console_scripts.py
--rw-r--r--  2.0 unx     7668 b- defN 20-Sep-09 09:08 integration_tests/test_ddd_py_to_xml.py
--rw-r--r--  2.0 unx     1241 b- defN 20-Sep-09 09:08 integration_tests/test_ddds.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/__init__.py
--rw-r--r--  2.0 unx    11134 b- defN 20-Sep-09 09:08 tala/config.py
--rw-r--r--  2.0 unx      116 b- defN 20-Sep-09 09:09 tala/installed_version.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/backend/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/backend/dependencies/__init__.py
--rw-r--r--  2.0 unx     3048 b- defN 20-Sep-09 09:08 tala/backend/dependencies/abstract_backend_dependencies.py
--rw-r--r--  2.0 unx     1605 b- defN 20-Sep-09 09:08 tala/backend/dependencies/for_generating.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/cli/__init__.py
--rw-r--r--  2.0 unx      877 b- defN 20-Sep-09 09:08 tala/cli/argument_parser.py
--rw-r--r--  2.0 unx      629 b- defN 20-Sep-09 09:08 tala/cli/console_formatting.py
--rw-r--r--  2.0 unx    14828 b- defN 20-Sep-09 09:08 tala/cli/console_script.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/cli/tdm/__init__.py
--rw-r--r--  2.0 unx      459 b- defN 20-Sep-09 09:08 tala/cli/tdm/passivity_timer.py
--rw-r--r--  2.0 unx     2800 b- defN 20-Sep-09 09:08 tala/cli/tdm/tdm_cli.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddd/__init__.py
--rw-r--r--  2.0 unx    20856 b- defN 20-Sep-09 09:08 tala/ddd/ddd_py_compiler.py
--rw-r--r--  2.0 unx    51241 b- defN 20-Sep-09 09:08 tala/ddd/ddd_xml_compiler.py
--rw-r--r--  2.0 unx    46160 b- defN 20-Sep-09 09:08 tala/ddd/parser.py
--rw-r--r--  2.0 unx     1428 b- defN 20-Sep-09 09:08 tala/ddd/utils.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddd/building/__init__.py
--rw-r--r--  2.0 unx     2713 b- defN 20-Sep-09 09:08 tala/ddd/building/ddd_builder_for_generating.py
--rw-r--r--  2.0 unx       94 b- defN 20-Sep-09 09:08 tala/ddd/building/supported_asrs.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddd/building/steps/__init__.py
--rw-r--r--  2.0 unx      522 b- defN 20-Sep-09 09:08 tala/ddd/building/steps/abstract_build_step.py
--rw-r--r--  2.0 unx     1497 b- defN 20-Sep-09 09:08 tala/ddd/building/steps/clean.py
--rw-r--r--  2.0 unx     2012 b- defN 20-Sep-09 09:08 tala/ddd/building/steps/generate.py
--rw-r--r--  2.0 unx     2967 b- defN 20-Sep-09 09:08 tala/ddd/building/steps/step_factory.py
--rw-r--r--  2.0 unx     2102 b- defN 20-Sep-09 09:08 tala/ddd/building/steps/verify.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddd/grammar/__init__.py
--rw-r--r--  2.0 unx      172 b- defN 20-Sep-09 09:08 tala/ddd/grammar/parser.py
--rw-r--r--  2.0 unx      762 b- defN 20-Sep-09 09:08 tala/ddd/grammar/reader.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddd/loading/__init__.py
--rw-r--r--  2.0 unx     5787 b- defN 20-Sep-09 09:08 tala/ddd/loading/ddd_loader.py
--rw-r--r--  2.0 unx     2496 b- defN 20-Sep-09 09:08 tala/ddd/loading/ddd_set_loader.py
--rw-r--r--  2.0 unx     2318 b- defN 20-Sep-09 09:08 tala/ddd/loading/python_module_loader.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddd/maker/__init__.py
--rw-r--r--  2.0 unx     4055 b- defN 20-Sep-09 09:08 tala/ddd/maker/ddd_maker.py
--rw-r--r--  2.0 unx    29722 b- defN 20-Sep-09 09:08 tala/ddd/maker/ddd_py_to_xml.py
--rw-r--r--  2.0 unx     1471 b- defN 20-Sep-09 09:08 tala/ddd/maker/utils.py
--rw-rw-r--  2.0 unx      221 b- defN 20-Sep-09 09:08 tala/ddd/maker/templates/domain_template.xml
--rw-rw-r--  2.0 unx       60 b- defN 20-Sep-09 09:08 tala/ddd/maker/templates/grammar_eng_template.xml
--rw-rw-r--  2.0 unx       44 b- defN 20-Sep-09 09:08 tala/ddd/maker/templates/interaction_tests_eng_template.txt
--rw-rw-r--  2.0 unx       85 b- defN 20-Sep-09 09:08 tala/ddd/maker/templates/ontology_template.xml
--rw-rw-r--  2.0 unx       80 b- defN 20-Sep-09 09:08 tala/ddd/maker/templates/service_interface_template.xml
--rw-rw-r--  2.0 unx      191 b- defN 20-Sep-09 09:08 tala/ddd/maker/templates/word_list_template.txt
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddd/schemas/__init__.py
--rw-rw-r--  2.0 unx    14080 b- defN 20-Sep-09 09:08 tala/ddd/schemas/domain.xsd
--rw-rw-r--  2.0 unx    11072 b- defN 20-Sep-09 09:08 tala/ddd/schemas/grammar.xsd
--rw-rw-r--  2.0 unx     6444 b- defN 20-Sep-09 09:08 tala/ddd/schemas/grammar_rgl.xsd
--rw-rw-r--  2.0 unx     1801 b- defN 20-Sep-09 09:08 tala/ddd/schemas/ontology.xsd
--rw-rw-r--  2.0 unx     7890 b- defN 20-Sep-09 09:08 tala/ddd/schemas/service_interface.xsd
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddd/services/__init__.py
--rw-r--r--  2.0 unx       55 b- defN 20-Sep-09 09:08 tala/ddd/services/constants.py
--rw-r--r--  2.0 unx    13020 b- defN 20-Sep-09 09:08 tala/ddd/services/service_interface.py
--rw-r--r--  2.0 unx     6017 b- defN 20-Sep-09 09:08 tala/ddd/services/service_interface_from_device.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/datetime_ddd/__init__.py
--rw-r--r--  2.0 unx      711 b- defN 20-Sep-09 09:08 tala/ddds/datetime_ddd/device.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/datetime_ddd/grammar/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/downdate_conditions/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/downdate_conditions/grammar/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/frontend_data_for_device/__init__.py
--rw-r--r--  2.0 unx     3102 b- defN 20-Sep-09 09:08 tala/ddds/frontend_data_for_device/device.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/frontend_data_for_device/grammar/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/frontend_data_for_http_service/__init__.py
--rw-r--r--  2.0 unx      170 b- defN 20-Sep-09 09:08 tala/ddds/frontend_data_for_http_service/device.py
--rw-r--r--  2.0 unx     6613 b- defN 20-Sep-09 09:08 tala/ddds/frontend_data_for_http_service/http_service.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/frontend_data_for_http_service/grammar/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/hello_world/__init__.py
--rw-r--r--  2.0 unx     1913 b- defN 20-Sep-09 09:08 tala/ddds/hello_world/device.py
--rw-r--r--  2.0 unx      717 b- defN 20-Sep-09 09:08 tala/ddds/hello_world/ontology.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/hello_world/grammar/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/http_service/__init__.py
--rw-r--r--  2.0 unx     4748 b- defN 20-Sep-09 09:08 tala/ddds/http_service/http_service.py
--rw-r--r--  2.0 unx      456 b- defN 20-Sep-09 09:08 tala/ddds/http_service/http_service_malformed_json.py
--rw-r--r--  2.0 unx      413 b- defN 20-Sep-09 09:08 tala/ddds/http_service/http_service_schema_violation.py
--rw-r--r--  2.0 unx      239 b- defN 20-Sep-09 09:08 tala/ddds/http_service/http_service_time_out.py
--rw-r--r--  2.0 unx      464 b- defN 20-Sep-09 09:08 tala/ddds/http_service/http_service_unexpected_status.py
--rw-r--r--  2.0 unx      207 b- defN 20-Sep-09 09:08 tala/ddds/http_service/http_service_unexpected_status_code.py
--rw-r--r--  2.0 unx      574 b- defN 20-Sep-09 09:08 tala/ddds/http_service/http_service_unexpected_version.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/http_service/grammar/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/incremental_search/__init__.py
--rw-r--r--  2.0 unx     4541 b- defN 20-Sep-09 09:08 tala/ddds/incremental_search/device.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/instructional/__init__.py
--rw-r--r--  2.0 unx     2229 b- defN 20-Sep-09 09:08 tala/ddds/instructional/http_service.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/instructional/grammar/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/mockup_travel/__init__.py
--rw-r--r--  2.0 unx     9877 b- defN 20-Sep-09 09:08 tala/ddds/mockup_travel/device.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/mockup_travel/grammar/__init__.py
--rw-r--r--  2.0 unx      288 b- defN 20-Sep-09 09:08 tala/ddds/mockup_travel/grammar/grammar_it.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/output_variation/__init__.py
--rw-r--r--  2.0 unx     1810 b- defN 20-Sep-09 09:08 tala/ddds/output_variation/device.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/output_variation/grammar/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/person_name/__init__.py
--rw-r--r--  2.0 unx      568 b- defN 20-Sep-09 09:08 tala/ddds/person_name/device.py
--rw-r--r--  2.0 unx     2507 b- defN 20-Sep-09 09:08 tala/ddds/person_name/http_service.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/person_name/grammar/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/phone_directory/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/phone_directory/grammar/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/rasa_answers/__init__.py
--rw-r--r--  2.0 unx      190 b- defN 20-Sep-09 09:08 tala/ddds/rasa_answers/device.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/rasa_answers/grammar/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/rasa_for_dynamic_entities/__init__.py
--rw-r--r--  2.0 unx     2255 b- defN 20-Sep-09 09:08 tala/ddds/rasa_for_dynamic_entities/device.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/rasa_for_dynamic_entities/grammar/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/rasa_for_rgl/__init__.py
--rw-r--r--  2.0 unx     3707 b- defN 20-Sep-09 09:08 tala/ddds/rasa_for_rgl/device.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/rasa_for_rgl/grammar/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/rasa_for_static_entities/__init__.py
--rw-r--r--  2.0 unx     1680 b- defN 20-Sep-09 09:08 tala/ddds/rasa_for_static_entities/device.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/rasa_for_static_entities/grammar/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/rasa_numbers/__init__.py
--rw-r--r--  2.0 unx      550 b- defN 20-Sep-09 09:08 tala/ddds/rasa_numbers/device.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/rasa_numbers/grammar/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/rasa_strings/__init__.py
--rw-r--r--  2.0 unx      188 b- defN 20-Sep-09 09:08 tala/ddds/rasa_strings/device.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/send_to_frontend/__init__.py
--rw-r--r--  2.0 unx     1765 b- defN 20-Sep-09 09:08 tala/ddds/send_to_frontend/device.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/send_to_frontend/grammar/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/small_grammar/__init__.py
--rw-r--r--  2.0 unx      273 b- defN 20-Sep-09 09:08 tala/ddds/small_grammar/service.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/small_grammar/grammar/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/tidePooler/__init__.py
--rw-r--r--  2.0 unx     2811 b- defN 20-Sep-09 09:08 tala/ddds/tidePooler/device.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/ddds/tidePooler/grammar/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/log/__init__.py
--rw-r--r--  2.0 unx     1557 b- defN 20-Sep-09 09:08 tala/log/logger.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/model/__init__.py
--rw-r--r--  2.0 unx     1320 b- defN 20-Sep-09 09:08 tala/model/action.py
--rw-r--r--  2.0 unx      259 b- defN 20-Sep-09 09:08 tala/model/action_status.py
--rw-r--r--  2.0 unx      215 b- defN 20-Sep-09 09:08 tala/model/ask_feature.py
--rw-r--r--  2.0 unx      910 b- defN 20-Sep-09 09:08 tala/model/audio_directive.py
--rw-r--r--  2.0 unx      287 b- defN 20-Sep-09 09:08 tala/model/common.py
--rw-r--r--  2.0 unx     1793 b- defN 20-Sep-09 09:08 tala/model/condition.py
--rw-r--r--  2.0 unx      506 b- defN 20-Sep-09 09:08 tala/model/database.py
--rw-r--r--  2.0 unx     1395 b- defN 20-Sep-09 09:08 tala/model/date_time.py
--rw-r--r--  2.0 unx     1755 b- defN 20-Sep-09 09:08 tala/model/ddd.py
--rw-r--r--  2.0 unx     3447 b- defN 20-Sep-09 09:08 tala/model/device.py
--rw-r--r--  2.0 unx    14070 b- defN 20-Sep-09 09:08 tala/model/domain.py
--rw-r--r--  2.0 unx      952 b- defN 20-Sep-09 09:08 tala/model/entity.py
--rw-r--r--  2.0 unx       82 b- defN 20-Sep-09 09:08 tala/model/error.py
--rw-r--r--  2.0 unx     1069 b- defN 20-Sep-09 09:08 tala/model/event_notification.py
--rw-r--r--  2.0 unx     5324 b- defN 20-Sep-09 09:08 tala/model/goal.py
--rw-r--r--  2.0 unx      549 b- defN 20-Sep-09 09:08 tala/model/image.py
--rw-r--r--  2.0 unx     3566 b- defN 20-Sep-09 09:08 tala/model/individual.py
--rw-r--r--  2.0 unx      766 b- defN 20-Sep-09 09:08 tala/model/input_hypothesis.py
--rw-r--r--  2.0 unx     2281 b- defN 20-Sep-09 09:08 tala/model/interpretation.py
--rw-r--r--  2.0 unx     2643 b- defN 20-Sep-09 09:08 tala/model/lambda_abstraction.py
--rw-r--r--  2.0 unx    20382 b- defN 20-Sep-09 09:08 tala/model/move.py
--rw-r--r--  2.0 unx    10528 b- defN 20-Sep-09 09:08 tala/model/ontology.py
--rw-r--r--  2.0 unx     4461 b- defN 20-Sep-09 09:08 tala/model/openqueue.py
--rw-r--r--  2.0 unx      352 b- defN 20-Sep-09 09:08 tala/model/person_name.py
--rw-r--r--  2.0 unx     2987 b- defN 20-Sep-09 09:08 tala/model/plan.py
--rw-r--r--  2.0 unx    15493 b- defN 20-Sep-09 09:08 tala/model/plan_item.py
--rw-r--r--  2.0 unx       48 b- defN 20-Sep-09 09:08 tala/model/polarity.py
--rw-r--r--  2.0 unx     1795 b- defN 20-Sep-09 09:08 tala/model/predicate.py
--rw-r--r--  2.0 unx    26904 b- defN 20-Sep-09 09:08 tala/model/proposition.py
--rw-r--r--  2.0 unx     3795 b- defN 20-Sep-09 09:08 tala/model/question.py
--rw-r--r--  2.0 unx     3390 b- defN 20-Sep-09 09:08 tala/model/question_raising_plan_item.py
--rw-r--r--  2.0 unx     1980 b- defN 20-Sep-09 09:08 tala/model/semantic_object.py
--rw-r--r--  2.0 unx     1254 b- defN 20-Sep-09 09:08 tala/model/service_action_outcome.py
--rw-r--r--  2.0 unx      229 b- defN 20-Sep-09 09:08 tala/model/service_invocation.py
--rw-r--r--  2.0 unx      485 b- defN 20-Sep-09 09:08 tala/model/service_query_result.py
--rw-r--r--  2.0 unx     2865 b- defN 20-Sep-09 09:08 tala/model/set.py
--rw-r--r--  2.0 unx     9737 b- defN 20-Sep-09 09:08 tala/model/sort.py
--rw-r--r--  2.0 unx       67 b- defN 20-Sep-09 09:08 tala/model/speaker.py
--rw-r--r--  2.0 unx     3840 b- defN 20-Sep-09 09:08 tala/model/stack.py
--rw-r--r--  2.0 unx      137 b- defN 20-Sep-09 09:08 tala/model/third_party_parser.py
--rw-r--r--  2.0 unx     1288 b- defN 20-Sep-09 09:08 tala/model/tis_node.py
--rw-r--r--  2.0 unx     2525 b- defN 20-Sep-09 09:08 tala/model/user_move.py
--rw-r--r--  2.0 unx     1318 b- defN 20-Sep-09 09:08 tala/model/validation_result.py
--rw-r--r--  2.0 unx      553 b- defN 20-Sep-09 09:08 tala/model/webview.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/model/grammar/__init__.py
--rw-r--r--  2.0 unx    12825 b- defN 20-Sep-09 09:08 tala/model/grammar/grammar.py
--rw-r--r--  2.0 unx     2329 b- defN 20-Sep-09 09:08 tala/model/grammar/intent.py
--rw-r--r--  2.0 unx      788 b- defN 20-Sep-09 09:08 tala/model/grammar/required_entity.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/nl/__init__.py
--rw-r--r--  2.0 unx     5802 b- defN 20-Sep-09 09:08 tala/nl/abstract_generator.py
--rw-r--r--  2.0 unx      409 b- defN 20-Sep-09 09:08 tala/nl/constants.py
--rw-r--r--  2.0 unx    19298 b- defN 20-Sep-09 09:08 tala/nl/examples.py
--rw-r--r--  2.0 unx      516 b- defN 20-Sep-09 09:08 tala/nl/generated_intent.py
--rw-r--r--  2.0 unx      531 b- defN 20-Sep-09 09:08 tala/nl/languages.py
--rw-r--r--  2.0 unx       40 b- defN 20-Sep-09 09:08 tala/nl/selection_policy_names.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/nl/alexa/__init__.py
--rw-r--r--  2.0 unx     7919 b- defN 20-Sep-09 09:08 tala/nl/alexa/generator.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/nl/gf/__init__.py
--rw-r--r--  2.0 unx    76716 b- defN 20-Sep-09 09:08 tala/nl/gf/auto_generator.py
--rw-r--r--  2.0 unx     2742 b- defN 20-Sep-09 09:08 tala/nl/gf/grammar_entry_types.py
--rw-r--r--  2.0 unx      322 b- defN 20-Sep-09 09:08 tala/nl/gf/naming.py
--rw-r--r--  2.0 unx      538 b- defN 20-Sep-09 09:08 tala/nl/gf/resource.py
--rw-r--r--  2.0 unx      164 b- defN 20-Sep-09 09:08 tala/nl/gf/resource_eng.py
--rw-r--r--  2.0 unx      460 b- defN 20-Sep-09 09:08 tala/nl/gf/resource_it.py
--rw-r--r--  2.0 unx       98 b- defN 20-Sep-09 09:08 tala/nl/gf/resource_sv.py
--rw-r--r--  2.0 unx    51072 b- defN 20-Sep-09 09:08 tala/nl/gf/rgl_gf_generator.py
--rw-r--r--  2.0 unx      222 b- defN 20-Sep-09 09:08 tala/nl/gf/rgl_grammar_entry_types.py
--rw-r--r--  2.0 unx     5162 b- defN 20-Sep-09 09:08 tala/nl/gf/utils.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/nl/rasa/__init__.py
--rw-r--r--  2.0 unx    10474 b- defN 20-Sep-09 09:08 tala/nl/rasa/generator.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/testing/__init__.py
--rw-r--r--  2.0 unx     2168 b- defN 20-Sep-09 09:08 tala/testing/backend_dependencies_test_base.py
--rw-r--r--  2.0 unx     3698 b- defN 20-Sep-09 09:08 tala/testing/ddd_mocker.py
--rw-r--r--  2.0 unx     6991 b- defN 20-Sep-09 09:08 tala/testing/lib_test_case.py
--rw-r--r--  2.0 unx     4750 b- defN 20-Sep-09 09:08 tala/testing/move_factory.py
--rw-r--r--  2.0 unx      517 b- defN 20-Sep-09 09:08 tala/testing/utils.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/testing/endurance/__init__.py
--rw-r--r--  2.0 unx     1958 b- defN 20-Sep-09 09:08 tala/testing/endurance/named_test.py
--rw-r--r--  2.0 unx     1488 b- defN 20-Sep-09 09:08 tala/testing/endurance/runner.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/testing/interactions/__init__.py
--rw-r--r--  2.0 unx      411 b- defN 20-Sep-09 09:08 tala/testing/interactions/base_test.py
--rw-r--r--  2.0 unx     8400 b- defN 20-Sep-09 09:08 tala/testing/interactions/compiler.py
--rw-r--r--  2.0 unx     1840 b- defN 20-Sep-09 09:08 tala/testing/interactions/file.py
--rw-r--r--  2.0 unx      466 b- defN 20-Sep-09 09:08 tala/testing/interactions/named_test.py
--rw-r--r--  2.0 unx      946 b- defN 20-Sep-09 09:08 tala/testing/interactions/result.py
--rw-r--r--  2.0 unx      219 b- defN 20-Sep-09 09:08 tala/testing/interactions/suite.py
--rw-r--r--  2.0 unx    12028 b- defN 20-Sep-09 09:08 tala/testing/interactions/testcase.py
--rw-r--r--  2.0 unx      679 b- defN 20-Sep-09 09:08 tala/testing/interactions/testloader.py
--rw-r--r--  2.0 unx     3654 b- defN 20-Sep-09 09:08 tala/testing/interactions/turn.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-09 09:08 tala/utils/__init__.py
--rw-r--r--  2.0 unx     1448 b- defN 20-Sep-09 09:08 tala/utils/as_json.py
--rw-r--r--  2.0 unx      104 b- defN 20-Sep-09 09:08 tala/utils/as_semantic_expression.py
--rw-r--r--  2.0 unx      676 b- defN 20-Sep-09 09:08 tala/utils/await_endpoint.py
--rw-r--r--  2.0 unx      383 b- defN 20-Sep-09 09:08 tala/utils/chdir.py
--rw-r--r--  2.0 unx      917 b- defN 20-Sep-09 09:08 tala/utils/equality.py
--rw-r--r--  2.0 unx      612 b- defN 20-Sep-09 09:08 tala/utils/float_comparison.py
--rw-r--r--  2.0 unx      466 b- defN 20-Sep-09 09:08 tala/utils/observable.py
--rw-r--r--  2.0 unx     5625 b- defN 20-Sep-09 09:08 tala/utils/tdm_client.py
--rw-r--r--  2.0 unx     1034 b- defN 20-Sep-09 09:08 tala/utils/unicodify.py
--rw-r--r--  2.0 unx      108 b- defN 20-Sep-09 09:08 tala/utils/unique.py
--rw-r--r--  2.0 unx     1301 b- defN 20-Sep-09 09:09 tala-8.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 20-Sep-09 09:09 tala-8.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 20-Sep-09 09:09 tala-8.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       27 b- defN 20-Sep-09 09:09 tala-8.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    20920 b- defN 20-Sep-09 09:09 tala-8.0.0.dist-info/RECORD
-238 files, 814658 bytes uncompressed, 173313 bytes compressed:  78.7%
+Zip file size: 219744 bytes, number of entries: 249
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 bin/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 integration_tests/__init__.py
+-rw-r--r--  2.0 unx     5995 b- defN 20-Oct-22 08:46 integration_tests/console_script_mixin.py
+-rw-r--r--  2.0 unx     9007 b- defN 20-Oct-22 08:46 integration_tests/expected_generate_rasa_output.py
+-rw-r--r--  2.0 unx     4937 b- defN 20-Oct-22 08:46 integration_tests/test_create_configs.py
+-rw-r--r--  2.0 unx      983 b- defN 20-Oct-22 08:46 integration_tests/test_create_ddd.py
+-rw-r--r--  2.0 unx     7668 b- defN 20-Oct-22 08:46 integration_tests/test_ddd_py_to_xml.py
+-rw-r--r--  2.0 unx     1241 b- defN 20-Oct-22 08:46 integration_tests/test_ddds.py
+-rw-r--r--  2.0 unx     8571 b- defN 20-Oct-22 08:46 integration_tests/test_generate_alexa.py
+-rw-r--r--  2.0 unx     6969 b- defN 20-Oct-22 08:46 integration_tests/test_generate_rasa.py
+-rw-r--r--  2.0 unx      555 b- defN 20-Oct-22 08:46 integration_tests/test_interact.py
+-rw-r--r--  2.0 unx     4296 b- defN 20-Oct-22 08:46 integration_tests/test_verify.py
+-rw-r--r--  2.0 unx     1053 b- defN 20-Oct-22 08:46 integration_tests/test_version.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/__init__.py
+-rw-r--r--  2.0 unx    11134 b- defN 20-Oct-22 08:46 tala/config.py
+-rw-r--r--  2.0 unx      116 b- defN 20-Oct-22 08:48 tala/installed_version.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/backend/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/backend/dependencies/__init__.py
+-rw-r--r--  2.0 unx     3048 b- defN 20-Oct-22 08:46 tala/backend/dependencies/abstract_backend_dependencies.py
+-rw-r--r--  2.0 unx     1605 b- defN 20-Oct-22 08:46 tala/backend/dependencies/for_generating.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/cli/__init__.py
+-rw-r--r--  2.0 unx      877 b- defN 20-Oct-22 08:46 tala/cli/argument_parser.py
+-rw-r--r--  2.0 unx      629 b- defN 20-Oct-22 08:46 tala/cli/console_formatting.py
+-rw-r--r--  2.0 unx    15691 b- defN 20-Oct-22 08:46 tala/cli/console_script.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/cli/tdm/__init__.py
+-rw-r--r--  2.0 unx      459 b- defN 20-Oct-22 08:46 tala/cli/tdm/passivity_timer.py
+-rw-r--r--  2.0 unx     2800 b- defN 20-Oct-22 08:46 tala/cli/tdm/tdm_cli.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddd/__init__.py
+-rw-r--r--  2.0 unx    20856 b- defN 20-Oct-22 08:46 tala/ddd/ddd_py_compiler.py
+-rw-r--r--  2.0 unx    51080 b- defN 20-Oct-22 08:46 tala/ddd/ddd_xml_compiler.py
+-rw-r--r--  2.0 unx    46752 b- defN 20-Oct-22 08:46 tala/ddd/parser.py
+-rw-r--r--  2.0 unx     1428 b- defN 20-Oct-22 08:46 tala/ddd/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddd/building/__init__.py
+-rw-r--r--  2.0 unx     2713 b- defN 20-Oct-22 08:46 tala/ddd/building/ddd_builder_for_generating.py
+-rw-r--r--  2.0 unx       94 b- defN 20-Oct-22 08:46 tala/ddd/building/supported_asrs.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddd/building/steps/__init__.py
+-rw-r--r--  2.0 unx      522 b- defN 20-Oct-22 08:46 tala/ddd/building/steps/abstract_build_step.py
+-rw-r--r--  2.0 unx     1497 b- defN 20-Oct-22 08:46 tala/ddd/building/steps/clean.py
+-rw-r--r--  2.0 unx     2012 b- defN 20-Oct-22 08:46 tala/ddd/building/steps/generate.py
+-rw-r--r--  2.0 unx     2967 b- defN 20-Oct-22 08:46 tala/ddd/building/steps/step_factory.py
+-rw-r--r--  2.0 unx     2102 b- defN 20-Oct-22 08:46 tala/ddd/building/steps/verify.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddd/grammar/__init__.py
+-rw-r--r--  2.0 unx      172 b- defN 20-Oct-22 08:46 tala/ddd/grammar/parser.py
+-rw-r--r--  2.0 unx      762 b- defN 20-Oct-22 08:46 tala/ddd/grammar/reader.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddd/loading/__init__.py
+-rw-r--r--  2.0 unx     5787 b- defN 20-Oct-22 08:46 tala/ddd/loading/ddd_loader.py
+-rw-r--r--  2.0 unx     2496 b- defN 20-Oct-22 08:46 tala/ddd/loading/ddd_set_loader.py
+-rw-r--r--  2.0 unx     2318 b- defN 20-Oct-22 08:46 tala/ddd/loading/python_module_loader.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddd/maker/__init__.py
+-rw-r--r--  2.0 unx     4055 b- defN 20-Oct-22 08:46 tala/ddd/maker/ddd_maker.py
+-rw-r--r--  2.0 unx    29722 b- defN 20-Oct-22 08:46 tala/ddd/maker/ddd_py_to_xml.py
+-rw-r--r--  2.0 unx     1471 b- defN 20-Oct-22 08:46 tala/ddd/maker/utils.py
+-rw-rw-r--  2.0 unx      221 b- defN 20-Oct-22 08:46 tala/ddd/maker/templates/domain_template.xml
+-rw-rw-r--  2.0 unx       60 b- defN 20-Oct-22 08:46 tala/ddd/maker/templates/grammar_eng_template.xml
+-rw-rw-r--  2.0 unx       44 b- defN 20-Oct-22 08:46 tala/ddd/maker/templates/interaction_tests_eng_template.txt
+-rw-rw-r--  2.0 unx       85 b- defN 20-Oct-22 08:46 tala/ddd/maker/templates/ontology_template.xml
+-rw-rw-r--  2.0 unx       80 b- defN 20-Oct-22 08:46 tala/ddd/maker/templates/service_interface_template.xml
+-rw-rw-r--  2.0 unx      191 b- defN 20-Oct-22 08:46 tala/ddd/maker/templates/word_list_template.txt
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddd/schemas/__init__.py
+-rw-rw-r--  2.0 unx    14130 b- defN 20-Oct-22 08:46 tala/ddd/schemas/domain.xsd
+-rw-rw-r--  2.0 unx    11072 b- defN 20-Oct-22 08:46 tala/ddd/schemas/grammar.xsd
+-rw-rw-r--  2.0 unx     6444 b- defN 20-Oct-22 08:46 tala/ddd/schemas/grammar_rgl.xsd
+-rw-rw-r--  2.0 unx     1801 b- defN 20-Oct-22 08:46 tala/ddd/schemas/ontology.xsd
+-rw-rw-r--  2.0 unx     7890 b- defN 20-Oct-22 08:46 tala/ddd/schemas/service_interface.xsd
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddd/services/__init__.py
+-rw-r--r--  2.0 unx       55 b- defN 20-Oct-22 08:46 tala/ddd/services/constants.py
+-rw-r--r--  2.0 unx    13020 b- defN 20-Oct-22 08:46 tala/ddd/services/service_interface.py
+-rw-r--r--  2.0 unx     6017 b- defN 20-Oct-22 08:46 tala/ddd/services/service_interface_from_device.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/datetime_ddd/__init__.py
+-rw-r--r--  2.0 unx      711 b- defN 20-Oct-22 08:46 tala/ddds/datetime_ddd/device.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/datetime_ddd/grammar/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/downdate_conditions/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/downdate_conditions/grammar/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/frontend_data_for_device/__init__.py
+-rw-r--r--  2.0 unx     3102 b- defN 20-Oct-22 08:46 tala/ddds/frontend_data_for_device/device.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/frontend_data_for_device/grammar/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/frontend_data_for_http_service/__init__.py
+-rw-r--r--  2.0 unx      170 b- defN 20-Oct-22 08:46 tala/ddds/frontend_data_for_http_service/device.py
+-rw-r--r--  2.0 unx     6613 b- defN 20-Oct-22 08:46 tala/ddds/frontend_data_for_http_service/http_service.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/frontend_data_for_http_service/grammar/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/hello_world/__init__.py
+-rw-r--r--  2.0 unx     1913 b- defN 20-Oct-22 08:46 tala/ddds/hello_world/device.py
+-rw-r--r--  2.0 unx      717 b- defN 20-Oct-22 08:46 tala/ddds/hello_world/ontology.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/hello_world/grammar/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/http_service/__init__.py
+-rw-r--r--  2.0 unx     4748 b- defN 20-Oct-22 08:46 tala/ddds/http_service/http_service.py
+-rw-r--r--  2.0 unx      456 b- defN 20-Oct-22 08:46 tala/ddds/http_service/http_service_malformed_json.py
+-rw-r--r--  2.0 unx      413 b- defN 20-Oct-22 08:46 tala/ddds/http_service/http_service_schema_violation.py
+-rw-r--r--  2.0 unx      239 b- defN 20-Oct-22 08:46 tala/ddds/http_service/http_service_time_out.py
+-rw-r--r--  2.0 unx      464 b- defN 20-Oct-22 08:46 tala/ddds/http_service/http_service_unexpected_status.py
+-rw-r--r--  2.0 unx      207 b- defN 20-Oct-22 08:46 tala/ddds/http_service/http_service_unexpected_status_code.py
+-rw-r--r--  2.0 unx      574 b- defN 20-Oct-22 08:46 tala/ddds/http_service/http_service_unexpected_version.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/http_service/grammar/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/incremental_search/__init__.py
+-rw-r--r--  2.0 unx     4541 b- defN 20-Oct-22 08:46 tala/ddds/incremental_search/device.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/instructional/__init__.py
+-rw-r--r--  2.0 unx     2229 b- defN 20-Oct-22 08:46 tala/ddds/instructional/http_service.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/instructional/grammar/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/mockup_travel/__init__.py
+-rw-r--r--  2.0 unx     9877 b- defN 20-Oct-22 08:46 tala/ddds/mockup_travel/device.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/mockup_travel/grammar/__init__.py
+-rw-r--r--  2.0 unx      288 b- defN 20-Oct-22 08:46 tala/ddds/mockup_travel/grammar/grammar_it.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/output_variation/__init__.py
+-rw-r--r--  2.0 unx     1810 b- defN 20-Oct-22 08:46 tala/ddds/output_variation/device.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/output_variation/grammar/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/person_name/__init__.py
+-rw-r--r--  2.0 unx      568 b- defN 20-Oct-22 08:46 tala/ddds/person_name/device.py
+-rw-r--r--  2.0 unx     2507 b- defN 20-Oct-22 08:46 tala/ddds/person_name/http_service.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/person_name/grammar/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/phone_directory/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/phone_directory/grammar/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/rasa_answers/__init__.py
+-rw-r--r--  2.0 unx      190 b- defN 20-Oct-22 08:46 tala/ddds/rasa_answers/device.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/rasa_answers/grammar/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/rasa_for_dynamic_entities/__init__.py
+-rw-r--r--  2.0 unx     2255 b- defN 20-Oct-22 08:46 tala/ddds/rasa_for_dynamic_entities/device.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/rasa_for_dynamic_entities/grammar/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/rasa_for_rgl/__init__.py
+-rw-r--r--  2.0 unx     3707 b- defN 20-Oct-22 08:46 tala/ddds/rasa_for_rgl/device.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/rasa_for_rgl/grammar/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/rasa_for_static_entities/__init__.py
+-rw-r--r--  2.0 unx     1680 b- defN 20-Oct-22 08:46 tala/ddds/rasa_for_static_entities/device.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/rasa_for_static_entities/grammar/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/rasa_numbers/__init__.py
+-rw-r--r--  2.0 unx      550 b- defN 20-Oct-22 08:46 tala/ddds/rasa_numbers/device.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/rasa_numbers/grammar/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/rasa_strings/__init__.py
+-rw-r--r--  2.0 unx      188 b- defN 20-Oct-22 08:46 tala/ddds/rasa_strings/device.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/send_to_frontend/__init__.py
+-rw-r--r--  2.0 unx     1765 b- defN 20-Oct-22 08:46 tala/ddds/send_to_frontend/device.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/send_to_frontend/grammar/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/small_grammar/__init__.py
+-rw-r--r--  2.0 unx      273 b- defN 20-Oct-22 08:46 tala/ddds/small_grammar/service.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/small_grammar/grammar/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/tidePooler/__init__.py
+-rw-r--r--  2.0 unx     2811 b- defN 20-Oct-22 08:46 tala/ddds/tidePooler/device.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/ddds/tidePooler/grammar/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/log/__init__.py
+-rw-r--r--  2.0 unx     2866 b- defN 20-Oct-22 08:46 tala/log/extractor.py
+-rw-r--r--  2.0 unx     9492 b- defN 20-Oct-22 08:46 tala/log/interaction_test_extractor.py
+-rw-r--r--  2.0 unx     1557 b- defN 20-Oct-22 08:46 tala/log/logger.py
+-rw-r--r--  2.0 unx      168 b- defN 20-Oct-22 08:46 tala/log/serialization.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/model/__init__.py
+-rw-r--r--  2.0 unx     1320 b- defN 20-Oct-22 08:46 tala/model/action.py
+-rw-r--r--  2.0 unx      370 b- defN 20-Oct-22 08:46 tala/model/action_status.py
+-rw-r--r--  2.0 unx      215 b- defN 20-Oct-22 08:46 tala/model/ask_feature.py
+-rw-r--r--  2.0 unx      910 b- defN 20-Oct-22 08:46 tala/model/audio_directive.py
+-rw-r--r--  2.0 unx      287 b- defN 20-Oct-22 08:46 tala/model/common.py
+-rw-r--r--  2.0 unx     1793 b- defN 20-Oct-22 08:46 tala/model/condition.py
+-rw-r--r--  2.0 unx      506 b- defN 20-Oct-22 08:46 tala/model/database.py
+-rw-r--r--  2.0 unx     1395 b- defN 20-Oct-22 08:46 tala/model/date_time.py
+-rw-r--r--  2.0 unx     1755 b- defN 20-Oct-22 08:46 tala/model/ddd.py
+-rw-r--r--  2.0 unx     3447 b- defN 20-Oct-22 08:46 tala/model/device.py
+-rw-r--r--  2.0 unx    14070 b- defN 20-Oct-22 08:46 tala/model/domain.py
+-rw-r--r--  2.0 unx      952 b- defN 20-Oct-22 08:46 tala/model/entity.py
+-rw-r--r--  2.0 unx       82 b- defN 20-Oct-22 08:46 tala/model/error.py
+-rw-r--r--  2.0 unx     1069 b- defN 20-Oct-22 08:46 tala/model/event_notification.py
+-rw-r--r--  2.0 unx     5324 b- defN 20-Oct-22 08:46 tala/model/goal.py
+-rw-r--r--  2.0 unx      549 b- defN 20-Oct-22 08:46 tala/model/image.py
+-rw-r--r--  2.0 unx     3566 b- defN 20-Oct-22 08:46 tala/model/individual.py
+-rw-r--r--  2.0 unx      950 b- defN 20-Oct-22 08:46 tala/model/input_hypothesis.py
+-rw-r--r--  2.0 unx     2551 b- defN 20-Oct-22 08:46 tala/model/interpretation.py
+-rw-r--r--  2.0 unx     2643 b- defN 20-Oct-22 08:46 tala/model/lambda_abstraction.py
+-rw-r--r--  2.0 unx    20373 b- defN 20-Oct-22 08:46 tala/model/move.py
+-rw-r--r--  2.0 unx    10528 b- defN 20-Oct-22 08:46 tala/model/ontology.py
+-rw-r--r--  2.0 unx     6821 b- defN 20-Oct-22 08:46 tala/model/openqueue.py
+-rw-r--r--  2.0 unx      352 b- defN 20-Oct-22 08:46 tala/model/person_name.py
+-rw-r--r--  2.0 unx     3411 b- defN 20-Oct-22 08:46 tala/model/plan.py
+-rw-r--r--  2.0 unx    16223 b- defN 20-Oct-22 08:46 tala/model/plan_item.py
+-rw-r--r--  2.0 unx       48 b- defN 20-Oct-22 08:46 tala/model/polarity.py
+-rw-r--r--  2.0 unx     1795 b- defN 20-Oct-22 08:46 tala/model/predicate.py
+-rw-r--r--  2.0 unx    27132 b- defN 20-Oct-22 08:46 tala/model/proposition.py
+-rw-r--r--  2.0 unx     3795 b- defN 20-Oct-22 08:46 tala/model/question.py
+-rw-r--r--  2.0 unx     3390 b- defN 20-Oct-22 08:46 tala/model/question_raising_plan_item.py
+-rw-r--r--  2.0 unx     1980 b- defN 20-Oct-22 08:46 tala/model/semantic_object.py
+-rw-r--r--  2.0 unx     1254 b- defN 20-Oct-22 08:46 tala/model/service_action_outcome.py
+-rw-r--r--  2.0 unx      229 b- defN 20-Oct-22 08:46 tala/model/service_invocation.py
+-rw-r--r--  2.0 unx      485 b- defN 20-Oct-22 08:46 tala/model/service_query_result.py
+-rw-r--r--  2.0 unx     2865 b- defN 20-Oct-22 08:46 tala/model/set.py
+-rw-r--r--  2.0 unx     9737 b- defN 20-Oct-22 08:46 tala/model/sort.py
+-rw-r--r--  2.0 unx       67 b- defN 20-Oct-22 08:46 tala/model/speaker.py
+-rw-r--r--  2.0 unx     3840 b- defN 20-Oct-22 08:46 tala/model/stack.py
+-rw-r--r--  2.0 unx      137 b- defN 20-Oct-22 08:46 tala/model/third_party_parser.py
+-rw-r--r--  2.0 unx     1288 b- defN 20-Oct-22 08:46 tala/model/tis_node.py
+-rw-r--r--  2.0 unx     2525 b- defN 20-Oct-22 08:46 tala/model/user_move.py
+-rw-r--r--  2.0 unx     1318 b- defN 20-Oct-22 08:46 tala/model/validation_result.py
+-rw-r--r--  2.0 unx      553 b- defN 20-Oct-22 08:46 tala/model/webview.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/model/grammar/__init__.py
+-rw-r--r--  2.0 unx    12825 b- defN 20-Oct-22 08:46 tala/model/grammar/grammar.py
+-rw-r--r--  2.0 unx     2329 b- defN 20-Oct-22 08:46 tala/model/grammar/intent.py
+-rw-r--r--  2.0 unx      788 b- defN 20-Oct-22 08:46 tala/model/grammar/required_entity.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/nl/__init__.py
+-rw-r--r--  2.0 unx     5832 b- defN 20-Oct-22 08:46 tala/nl/abstract_generator.py
+-rw-r--r--  2.0 unx      409 b- defN 20-Oct-22 08:46 tala/nl/constants.py
+-rw-r--r--  2.0 unx    21934 b- defN 20-Oct-22 08:46 tala/nl/examples.py
+-rw-r--r--  2.0 unx     1181 b- defN 20-Oct-22 08:46 tala/nl/generated_intent.py
+-rw-r--r--  2.0 unx      531 b- defN 20-Oct-22 08:46 tala/nl/languages.py
+-rw-r--r--  2.0 unx       40 b- defN 20-Oct-22 08:46 tala/nl/selection_policy_names.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/nl/alexa/__init__.py
+-rw-r--r--  2.0 unx     7919 b- defN 20-Oct-22 08:46 tala/nl/alexa/generator.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/nl/gf/__init__.py
+-rw-r--r--  2.0 unx    76716 b- defN 20-Oct-22 08:46 tala/nl/gf/auto_generator.py
+-rw-r--r--  2.0 unx     2742 b- defN 20-Oct-22 08:46 tala/nl/gf/grammar_entry_types.py
+-rw-r--r--  2.0 unx      322 b- defN 20-Oct-22 08:46 tala/nl/gf/naming.py
+-rw-r--r--  2.0 unx      538 b- defN 20-Oct-22 08:46 tala/nl/gf/resource.py
+-rw-r--r--  2.0 unx      164 b- defN 20-Oct-22 08:46 tala/nl/gf/resource_eng.py
+-rw-r--r--  2.0 unx      460 b- defN 20-Oct-22 08:46 tala/nl/gf/resource_it.py
+-rw-r--r--  2.0 unx       98 b- defN 20-Oct-22 08:46 tala/nl/gf/resource_sv.py
+-rw-r--r--  2.0 unx    51072 b- defN 20-Oct-22 08:46 tala/nl/gf/rgl_gf_generator.py
+-rw-r--r--  2.0 unx      222 b- defN 20-Oct-22 08:46 tala/nl/gf/rgl_grammar_entry_types.py
+-rw-r--r--  2.0 unx     5162 b- defN 20-Oct-22 08:46 tala/nl/gf/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/nl/rasa/__init__.py
+-rw-r--r--  2.0 unx    10957 b- defN 20-Oct-22 08:46 tala/nl/rasa/generator.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/testing/__init__.py
+-rw-r--r--  2.0 unx     2168 b- defN 20-Oct-22 08:46 tala/testing/backend_dependencies_test_base.py
+-rw-r--r--  2.0 unx     3698 b- defN 20-Oct-22 08:46 tala/testing/ddd_mocker.py
+-rw-r--r--  2.0 unx     6991 b- defN 20-Oct-22 08:46 tala/testing/lib_test_case.py
+-rw-r--r--  2.0 unx     4750 b- defN 20-Oct-22 08:46 tala/testing/move_factory.py
+-rw-r--r--  2.0 unx      517 b- defN 20-Oct-22 08:46 tala/testing/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/testing/endurance/__init__.py
+-rw-r--r--  2.0 unx     1958 b- defN 20-Oct-22 08:46 tala/testing/endurance/named_test.py
+-rw-r--r--  2.0 unx     1488 b- defN 20-Oct-22 08:46 tala/testing/endurance/runner.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/testing/interactions/__init__.py
+-rw-r--r--  2.0 unx      411 b- defN 20-Oct-22 08:46 tala/testing/interactions/base_test.py
+-rw-r--r--  2.0 unx    10007 b- defN 20-Oct-22 08:46 tala/testing/interactions/compiler.py
+-rw-r--r--  2.0 unx     1840 b- defN 20-Oct-22 08:46 tala/testing/interactions/file.py
+-rw-r--r--  2.0 unx      466 b- defN 20-Oct-22 08:46 tala/testing/interactions/named_test.py
+-rw-r--r--  2.0 unx      946 b- defN 20-Oct-22 08:46 tala/testing/interactions/result.py
+-rw-r--r--  2.0 unx      219 b- defN 20-Oct-22 08:46 tala/testing/interactions/suite.py
+-rw-r--r--  2.0 unx    12957 b- defN 20-Oct-22 08:46 tala/testing/interactions/testcase.py
+-rw-r--r--  2.0 unx      679 b- defN 20-Oct-22 08:46 tala/testing/interactions/testloader.py
+-rw-r--r--  2.0 unx     4075 b- defN 20-Oct-22 08:46 tala/testing/interactions/turn.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Oct-22 08:46 tala/utils/__init__.py
+-rw-r--r--  2.0 unx     1448 b- defN 20-Oct-22 08:46 tala/utils/as_json.py
+-rw-r--r--  2.0 unx      104 b- defN 20-Oct-22 08:46 tala/utils/as_semantic_expression.py
+-rw-r--r--  2.0 unx      676 b- defN 20-Oct-22 08:46 tala/utils/await_endpoint.py
+-rw-r--r--  2.0 unx      383 b- defN 20-Oct-22 08:46 tala/utils/chdir.py
+-rw-r--r--  2.0 unx      917 b- defN 20-Oct-22 08:46 tala/utils/equality.py
+-rw-r--r--  2.0 unx      612 b- defN 20-Oct-22 08:46 tala/utils/float_comparison.py
+-rw-r--r--  2.0 unx      466 b- defN 20-Oct-22 08:46 tala/utils/observable.py
+-rw-r--r--  2.0 unx     5722 b- defN 20-Oct-22 08:46 tala/utils/tdm_client.py
+-rw-r--r--  2.0 unx     1034 b- defN 20-Oct-22 08:46 tala/utils/unicodify.py
+-rw-r--r--  2.0 unx      108 b- defN 20-Oct-22 08:46 tala/utils/unique.py
+-rw-r--r--  2.0 unx     1267 b- defN 20-Oct-22 08:48 tala-9.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 20-Oct-22 08:48 tala-9.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 20-Oct-22 08:48 tala-9.0.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       27 b- defN 20-Oct-22 08:48 tala-9.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    21933 b- defN 20-Oct-22 08:48 tala-9.0.0.dist-info/RECORD
+249 files, 851354 bytes uncompressed, 184672 bytes compressed:  78.3%
```

## zipnote {}

```diff
@@ -1,22 +1,46 @@
 Filename: bin/__init__.py
 Comment: 
 
 Filename: integration_tests/__init__.py
 Comment: 
 
-Filename: integration_tests/test_console_scripts.py
+Filename: integration_tests/console_script_mixin.py
+Comment: 
+
+Filename: integration_tests/expected_generate_rasa_output.py
+Comment: 
+
+Filename: integration_tests/test_create_configs.py
+Comment: 
+
+Filename: integration_tests/test_create_ddd.py
 Comment: 
 
 Filename: integration_tests/test_ddd_py_to_xml.py
 Comment: 
 
 Filename: integration_tests/test_ddds.py
 Comment: 
 
+Filename: integration_tests/test_generate_alexa.py
+Comment: 
+
+Filename: integration_tests/test_generate_rasa.py
+Comment: 
+
+Filename: integration_tests/test_interact.py
+Comment: 
+
+Filename: integration_tests/test_verify.py
+Comment: 
+
+Filename: integration_tests/test_version.py
+Comment: 
+
 Filename: tala/__init__.py
 Comment: 
 
 Filename: tala/config.py
 Comment: 
 
 Filename: tala/installed_version.py
@@ -387,17 +411,26 @@
 
 Filename: tala/ddds/tidePooler/grammar/__init__.py
 Comment: 
 
 Filename: tala/log/__init__.py
 Comment: 
 
+Filename: tala/log/extractor.py
+Comment: 
+
+Filename: tala/log/interaction_test_extractor.py
+Comment: 
+
 Filename: tala/log/logger.py
 Comment: 
 
+Filename: tala/log/serialization.py
+Comment: 
+
 Filename: tala/model/__init__.py
 Comment: 
 
 Filename: tala/model/action.py
 Comment: 
 
 Filename: tala/model/action_status.py
@@ -693,23 +726,23 @@
 
 Filename: tala/utils/unicodify.py
 Comment: 
 
 Filename: tala/utils/unique.py
 Comment: 
 
-Filename: tala-8.0.0.dist-info/METADATA
+Filename: tala-9.0.0.dist-info/METADATA
 Comment: 
 
-Filename: tala-8.0.0.dist-info/WHEEL
+Filename: tala-9.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: tala-8.0.0.dist-info/entry_points.txt
+Filename: tala-9.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: tala-8.0.0.dist-info/top_level.txt
+Filename: tala-9.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: tala-8.0.0.dist-info/RECORD
+Filename: tala-9.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tala/installed_version.py

```diff
@@ -1,4 +1,4 @@
 # coding: utf-8
 # file generated by setuptools_scm
 # don't change, don't track in version control
-version = '8.0.0'
+version = '9.0.0'
```

## tala/cli/console_script.py

```diff
@@ -21,14 +21,15 @@
 from tala.config import BackendConfig, DddConfig, DeploymentsConfig, BackendConfigNotFoundException, \
     DddConfigNotFoundException, DeploymentsConfigNotFoundException
 from tala.ddd.building.ddd_builder_for_generating import DDDBuilderForGenerating
 from tala.ddd.maker import utils as ddd_maker_utils
 from tala.ddd.maker.ddd_maker import DddMaker
 from tala import installed_version
 from tala.log.logger import configure_stdout_logging
+from tala.log.interaction_test_extractor import InteractionTestExtractor
 from tala.nl import languages
 from tala.nl.rasa.generator import RasaGenerator
 from tala.nl.alexa.generator import AlexaGenerator
 from tala.testing.interactions.file import InteractionTestingFile
 from tala.testing.interactions.testloader import InteractionTestingLoader
 from tala.testing.interactions.result import InteractionTestResult
 from tala.utils.tdm_client import TDMClient
@@ -246,14 +247,21 @@
 
     signal.signal(signal.SIGINT, on_terminate_signal)
     signal.signal(signal.SIGTERM, on_terminate_signal)
 
     test_runner.run()
 
 
+def extract(args):
+    extractor = InteractionTestExtractor.from_args(
+        args.log, verbose=args.verbose, full=args.full, semantic=args.semantic
+    )
+    extractor.run()
+
+
 def add_verify_subparser(subparsers):
     parser = subparsers.add_parser(
         "verify", help="verify the format of all DDDs supported by the backend, across all supported languages"
     )
     parser.set_defaults(func=verify)
     add_common_backend_arguments(parser)
     parser.add_argument(
@@ -380,14 +388,23 @@
         metavar="SECONDS",
         help="run until the duration has elapsed; if duration is 0, run forever"
     )
     parser.add_argument("--seed", type=int, metavar="INTEGER", help="random seed")
     parser.set_defaults(func=endurancetest)
 
 
+def add_extract_subparser(subparsers):
+    parser = subparsers.add_parser("extract", help="extract interaction test from a TDM log file")
+    parser.add_argument("-v", "--verbose", action="store_true", dest="verbose", help="print verbose information")
+    parser.add_argument("-f", "--full", action="store_true", help="print full interpretation information")
+    parser.add_argument("-s", "--semantic", action="store_true", help="print semantic information")
+    parser.set_defaults(func=extract)
+    parser.add_argument("log", help="the TDM session log to extract from")
+
+
 def format_warnings():
     def warning_on_one_line(message, category, _filename, _lineno, _file=None, _line=None):
         string = "%s: %s\n" % (category.__name__, message)
         return console_formatting.bold(string)
 
     warnings.formatwarning = warning_on_one_line
 
@@ -407,14 +424,15 @@
     add_create_backend_config_subparser(subparsers)
     add_create_ddd_config_subparser(subparsers)
     add_create_deployments_config_subparser(subparsers)
     add_version_subparser(subparsers)
     add_interact_subparser(subparsers)
     add_test_subparser(subparsers)
     add_endurancetest_subparser(subparsers)
+    add_extract_subparser(subparsers)
 
     parsed_args = root_parser.parse_args(args)
     with _config_exception_handling():
         parsed_args.func(parsed_args)
 
 
 if __name__ == "__main__":
```

## tala/ddd/ddd_xml_compiler.py

```diff
@@ -563,29 +563,25 @@
         speaker = Speaker.SYS
         speaker_attribute = element.getAttribute("speaker")
         if speaker_attribute == "user":
             speaker = Speaker.USR
         return GoalProposition(ResolveGoal(question, speaker))
 
     def _compile_if_then_child_plan(self, element, node_name):
-        nodes = self._find_child_nodes(element, node_name)
-        if len(nodes) == 0:
-            return None
-        elif len(nodes) == 1:
-            child_node = nodes[0]
-            if len(child_node.childNodes) == 0:
-                return None
+        def compile_then_or_else_node(then_or_else_node):
+            if len(then_or_else_node.childNodes) == 0:
+                return []
             else:
-                plan_items = self._compile_plan_item_nodes(child_node.childNodes)
-                if len(plan_items) == 0:
-                    return None
-                elif len(plan_items) == 1:
-                    return plan_items[0]
-                else:
-                    raise DddXmlCompilerException("if element only support single-item consequents and alternatives")
+                return self._compile_plan_item_nodes(then_or_else_node.childNodes)
+
+        then_or_else_nodes = self._find_child_nodes(element, node_name)
+        if len(then_or_else_nodes) == 0:
+            return []
+        elif len(then_or_else_nodes) == 1:
+            return compile_then_or_else_node(then_or_else_nodes[0])
         else:
             raise DddXmlCompilerException("expected only one %r element" % node_name)
 
     def _compile_plan_single_attribute(self, plan, element, attribute_name, compilation_method):
         attribute = element.getAttribute(attribute_name)
         if attribute:
             plan[attribute_name] = compilation_method(attribute)
```

## tala/ddd/parser.py

```diff
@@ -66,15 +66,14 @@
             self._parse_service_result_proposition,
             self._parse_successful_service_action,
             self._parse_failed_service_action,
             self._parse_action_status,
             self._parse_decorated_icm_move,
             self._parse_icm_move,
             self._parse_proposition,
-            self._parse_negative_individual,
             self._parse_yes_or_no,
             self._parse_prop_set,
             self._parse_action,
             self._parse_individual,
             self._parse_predicate,
             self._parse_string,
         ]
@@ -801,21 +800,21 @@
 
     def _parse_if_then_else_plan_item(self, string):
         m = re.search(r'^if (.+) then (.*) else (.*)$', string)
         if m:
             (condition_string, consequent_string, alternative_string) = m.groups()
             condition = self._parse_proposition(condition_string)
             if consequent_string != "":
-                consequent = self.parse(consequent_string)
+                consequent = [self.parse(consequent_string)]
             else:
-                consequent = None
+                consequent = []
             if alternative_string != "":
-                alternative = self.parse(alternative_string)
+                alternative = [self.parse(alternative_string)]
             else:
-                alternative = None
+                alternative = []
             return IfThenElse(condition, consequent, alternative)
         else:
             raise ParseFailure()
 
     def _parse_jumpto_plan_item(self, string):
         m = re.search(r'^jumpto\((.+)\)$', string)
         if m:
@@ -878,44 +877,53 @@
                     individual = None
                 else:
                     individual = self._parse_individual(individual_string)
                 polarity = self._parse_polarity(polarity_str)
                 return PredicateProposition(predicate, individual, polarity)
         raise ParseFailure()
 
-    def _parse_negative_individual(self, string):
-        m = re.search(r'^~(\w+)$', string)
-        if m:
-            individual_value = m.group(1)
-            return self.ontology.create_negative_individual(individual_value)
-        raise ParseFailure()
-
     def _parse_individual(self, string):
+        def negate_if_negative_polarity(individual, polarity):
+            if polarity is Polarity.NEG:
+                return individual.negate()
+            else:
+                return individual
+
+        m = re.search(r'^(~?)(.+)$', string)
+        polarity_string = m.group(1)
+        individual_string = m.group(2)
+        polarity = self._parse_polarity(polarity_string)
         try:
-            return self._parse_real_individual(string)
+            individual = self._parse_real_individual(individual_string)
+            return negate_if_negative_polarity(individual, polarity)
         except ParseFailure:
             pass
         try:
-            return self._parse_integer_individual(string)
+            individual = self._parse_integer_individual(individual_string)
+            return negate_if_negative_polarity(individual, polarity)
         except ParseFailure:
             pass
         try:
-            return self._parse_string_individual(string)
+            individual = self._parse_string_individual(individual_string)
+            return negate_if_negative_polarity(individual, polarity)
         except ParseFailure:
             pass
         try:
-            return self._parse_individual_of_enumerated_sort(string)
+            individual = self._parse_individual_of_enumerated_sort(individual_string)
+            return negate_if_negative_polarity(individual, polarity)
         except ParseFailure:
             pass
         try:
-            return self._parse_individual_of_person_name_sort(string)
+            individual = self._parse_individual_of_person_name_sort(individual_string)
+            return negate_if_negative_polarity(individual, polarity)
         except ParseFailure:
             pass
         try:
-            return self._parse_individual_of_datetime_sort(string)
+            individual = self._parse_individual_of_datetime_sort(individual_string)
+            return negate_if_negative_polarity(individual, polarity)
         except ParseFailure:
             pass
         raise ParseFailure()
 
     def _parse_individual_of_enumerated_sort(self, string):
         m = re.search(r'^(.+)$', string)
         if m:
```

## tala/ddd/schemas/domain.xsd

### tala/ddd/schemas/domain.xsd

```diff
@@ -111,16 +111,16 @@
       </xs:complexContent>
     </xs:complexType>
   </xs:element>
   <xs:element name="if">
     <xs:complexType>
       <xs:sequence>
         <xs:element name="condition" type="proposition"/>
-        <xs:element name="then" type="plan"/>
-        <xs:element name="else" type="plan"/>
+        <xs:element name="then" type="plan" minOccurs="0" maxOccurs="1"/>
+        <xs:element name="else" type="plan" minOccurs="0" maxOccurs="1"/>
       </xs:sequence>
     </xs:complexType>
   </xs:element>
   <xs:element name="invoke_service_action">
     <xs:annotation>
       <xs:documentation xml:lang="en">Note: The attribute 'device' is not supported. Use 'service_interface.xml' instead.</xs:documentation>
     </xs:annotation>
```

## tala/model/action_status.py

```diff
@@ -1,12 +1,20 @@
 from tala.model.semantic_object import SemanticObject
 
+DONE = "done"
+
 
 class Done(SemanticObject):
     def __eq__(self, other):
         return isinstance(other, Done)
 
     def as_semantic_expression(self):
-        return "done"
+        return DONE
 
     def __str__(self):
-        return "done"
+        return DONE
+
+    def __repr__(self):
+        return "Done()"
+
+    def __hash__(self):
+        return hash(DONE)
```

## tala/model/input_hypothesis.py

```diff
@@ -1,16 +1,24 @@
 from typing import Text  # noqa: F401
 
+from tala.utils.as_json import AsJSONMixin
 
-class InputHypothesis(object):
+
+class InputHypothesis(AsJSONMixin):
     def __init__(self, utterance, confidence):
         # type: (Text, float) -> None
         self._utterance = utterance
         self._confidence = confidence
 
+    def as_dict(self):
+        return {
+            "utterance": self.utterance,
+            "confidence": self.confidence,
+        }
+
     @property
     def utterance(self):
         # type: () -> Text
         return self._utterance
 
     @property
     def confidence(self):
```

## tala/model/interpretation.py

```diff
@@ -1,19 +1,20 @@
 from tala.model.common import Modality
 from tala.model.user_move import UserMove  # noqa: F401
+from tala.utils.as_json import AsJSONMixin
 from tala.utils.equality import EqualityMixin
 from tala.utils.unicodify import unicodify
 
 
 class UnexpectedModalityException(Exception):
     pass
 
 
-class Interpretation(EqualityMixin):
-    def __init__(self, moves, modality, utterance=None):
+class Interpretation(EqualityMixin, AsJSONMixin):
+    def __init__(self, moves, modality, utterance=None, perception_confidence=None):
         # type: ([UserMove], str, str) -> None
         self._moves = moves
         if modality not in Modality.SUPPORTED_MODALITIES:
             raise UnexpectedModalityException(
                 f"Expected one of the supported modalities {Modality.SUPPORTED_MODALITIES} but got '{modality}'"
             )
         if utterance:
@@ -22,14 +23,15 @@
                     f"Expected no utterance for modality '{modality}' but got '{utterance}'"
                 )
         if not utterance:
             if modality in Modality.REQUIRES_UTTERANCE:
                 raise UnexpectedModalityException(f"Expected an utterance for modality '{modality}' but it was missing")
         self._modality = modality
         self._utterance = utterance
+        self._perception_confidence = perception_confidence
 
     @property
     def moves(self):
         # type: () -> [UserMove]
         return self._moves
 
     @property
@@ -38,23 +40,27 @@
         return self._modality
 
     @property
     def utterance(self):
         # type: () -> str
         return self._utterance
 
+    @property
+    def perception_confidence(self):
+        return self._perception_confidence
+
     def as_dict(self):
         return {
             "modality": self.modality,
             "moves": [move.as_dict() for move in self.moves],
             "utterance": self.utterance,
         }
 
     def __repr__(self):
-        return f"{self.__class__.__name__}({unicodify(self._moves)}, {self._modality}, {self._utterance})"
+        return f"{self.__class__.__name__}({unicodify(self._moves)}, {self._modality}, {self._utterance}, {self._perception_confidence})"
 
 
 class InterpretationWithoutUtterance(Interpretation):
     def __init__(self, moves, modality):
         # type: ([UserMove], str) -> None
         super(InterpretationWithoutUtterance, self).__init__(moves, modality)
         self._moves = moves
```

## tala/model/move.py

```diff
@@ -80,15 +80,15 @@
 
     @property
     def perception_confidence(self):
         return self._perception_confidence
 
     @property
     def confidence(self):
-        confidence_sources = [self.perception_confidence, self.weighted_understanding_confidence]
+        confidence_sources = [self.perception_confidence, self.understanding_confidence]
         if None in confidence_sources:
             return None
         return self.perception_confidence * self.understanding_confidence
 
     @property
     def weighted_confidence(self):
         confidence_sources = [self.perception_confidence, self.weighted_understanding_confidence]
```

## tala/model/openqueue.py

```diff
@@ -1,17 +1,105 @@
 import copy
 
 from tala.utils.as_json import AsJSONMixin
 from tala.utils.unicodify import unicodify
+from tala.utils.equality import EqualityMixin
 
 
 class OpenQueueError(Exception):
     pass
 
 
+class Interpretation(AsJSONMixin, EqualityMixin):
+    def __init__(self, moves, utterance, default_perception_confidence):
+        self._moves = moves
+        self._utterance = utterance
+        self._default_perception_confidence = default_perception_confidence
+
+    def as_dict(self):
+        return self._moves.as_dict()
+
+    def enqueue(self, element):
+        self._moves.enqueue(element)
+
+    def enqueue_first(self, element):
+        self._moves.enqueue_first(element)
+
+    def first(self, element):
+        self._moves.first(element)
+
+    def is_first(self, element):
+        self._moves.is_first(element)
+
+    def last(self, element):
+        self._moves.last(element)
+
+    def dequeue(self):
+        self._moves.dequeue()
+
+    def remove(self, element):
+        self._moves.remove(element)
+
+    def remove_if_exists(self, element):
+        self._moves.remove_if_exists(element)
+
+    def clear(self):
+        self._moves.clear()
+
+    def shift(self):
+        self._moves.shift()
+
+    def init_shift(self):
+        self._moves.init_shift()
+
+    def cancel_shift(self):
+        self._moves.cancel_shift()
+
+    def fully_shifted(self):
+        self._moves.fully_shifted()
+
+    def is_shift_initialised(self):
+        self._moves.is_shifted_initiated()
+
+    def __len__(self):
+        return len(self._moves)
+
+    def __iter__(self):
+        return iter(self._moves)
+
+    def __getitem__(self, index):
+        return self._moves[index]
+
+    def __str__(self):
+        string = f'Interpretation({unicodify(self._moves)}, {unicodify(self.average_perception_confidence)})'
+        return string
+
+    def __repr__(self):
+        string = f'Interpretation({self._moves}, {self.average_perception_confidence})'
+        return string
+
+    @property
+    def utterance(self):
+        return self._utterance
+
+    @property
+    def average_weighted_confidence(self):
+        return sum([move.weighted_confidence for move in self._moves]) / len(self._moves)
+
+    @property
+    def average_perception_confidence(self):
+        if self._moves:
+            return sum([move.perception_confidence for move in self._moves]) / len(self._moves)
+        return self._default_perception_confidence
+
+    @property
+    def average_confidence(self):
+        return sum([move.confidence for move in self._moves]) / len(self._moves)
+
+
 class OpenQueue(AsJSONMixin):
     def __init__(self, iterable=None):
         super(OpenQueue, self).__init__()
         self.front_content = []
         self.back_content = []
         if iterable is not None:
             for item in iterable:
```

## tala/model/plan.py

```diff
@@ -46,35 +46,44 @@
     def __iter__(self):
         flattened_items = self._flatten(self.content)
         return flattened_items.__iter__()
 
     def _flatten(self, items):
         result = []
         for item in items:
-            if item.getType() == PlanItem.TYPE_IF_THEN_ELSE:
-                if item.consequent:
-                    result.append(item.get_consequent())
-                if item.alternative:
-                    result.append(item.get_alternative())
-            else:
-                result.append(item)
+            try:
+                if item.getType() == PlanItem.TYPE_IF_THEN_ELSE:
+                    if item.consequent:
+                        result.extend(item.get_consequent())
+                    if item.alternative:
+                        result.extend(item.get_alternative())
+                else:
+                    result.append(item)
+            except AttributeError:
+                result.extend(item)
         return result
 
     def remove(self, item_to_remove):
+        items_to_remove = []
         for item in self.content:
             if item == item_to_remove:
-                self.content.remove(item)
+                items_to_remove.append(item)
             elif item.getType() == PlanItem.TYPE_IF_THEN_ELSE:
                 self.remove_nested(item_to_remove, item)
+        for item in items_to_remove:
+            self.content.remove(item)
 
     def remove_nested(self, to_remove, plan_item):
-        if to_remove == plan_item.consequent:
-            plan_item.consequent = None
-        if to_remove == plan_item.alternative:
-            plan_item.alternative = None
+        if to_remove in plan_item.consequent:
+            plan_item.consequent.remove(to_remove)
+        if to_remove in plan_item.alternative:
+            plan_item.alternative.remove(to_remove)
+        for item in plan_item.alternative + plan_item.consequent:
+            if item.getType() == PlanItem.TYPE_IF_THEN_ELSE:
+                self.remove_nested(to_remove, item)
 
     def get_questions_in_plan_without_feature_question(self):
         for plan_item in self:
             if plan_item.is_question_plan_item():
                 question = plan_item.getContent()
                 yield question
```

## tala/model/plan_item.py

```diff
@@ -267,23 +267,36 @@
 
 
 class IfThenElse(PlanItem):
     def __init__(self, condition, consequent, alternative):
         self.condition = condition
         self.consequent = consequent
         self.alternative = alternative
-        assert consequent is not None or alternative is not None, "One of consequent (%s) and alternative (%s) must not be None" % (
-            consequent, alternative
-        )
-        if consequent is not None and alternative is not None:
-            assert consequent.ontology_name == alternative.ontology_name, "Expected identical ontologies in both consequent (%s) and alternative (%s) but got %r and %r" % (
-                consequent, alternative, consequent.ontology_name, alternative.ontology_name
-            )
+        self._check_integrity_of_data()
         PlanItem.__init__(self, PlanItem.TYPE_IF_THEN_ELSE)
 
+    def _check_integrity_of_data(self):
+        self._assert_one_alternative_is_non_empty_list()
+        self._assert_ontology_integrity()
+
+    def _assert_one_alternative_is_non_empty_list(self):
+        assert self.consequent is not [] or self.alternative is not [],\
+            "One of consequent (%s) and alternative (%s) must not be []" % (self.consequent, self.alternative)
+
+    def _assert_ontology_integrity(self):
+        if self.consequent is not [] or self.alternative is not []:
+            items = self.consequent + self.alternative
+            ontology_specific_plan_items = [item for item in items if item.is_ontology_specific()]
+            if len(ontology_specific_plan_items) > 0:
+                ontology_name = ontology_specific_plan_items[0].ontology_name
+                for item in ontology_specific_plan_items:
+                    assert ontology_name == item.ontology_name, "Expected identical ontologies in all consequents (%s) and alternatives (%s) but got %r and %r (plan item: %r)" % (
+                        self.consequent, self.alternative, ontology_name, item.ontology_name, item
+                    )
+
     def get_condition(self):
         return self.condition
 
     def get_consequent(self):
         return self.consequent
 
     def get_alternative(self):
@@ -292,15 +305,16 @@
     def remove_consequent(self):
         self.consequent = None
 
     def remove_alternative(self):
         self.alternative = None
 
     def __str__(self):
-        return "if_then_else{}".format(unicodify((self.condition, self.consequent, self.alternative)))
+        result = "if_then_else{}".format(unicodify((self.condition, self.consequent, self.alternative)))
+        return result
 
     def as_dict(self):
         return {
             self.get_type(): {
                 "condition": self.condition,
                 "consequent": self.consequent,
                 "alternative": self.alternative,
@@ -474,11 +488,14 @@
     @property
     def message(self):
         return self._message
 
     def __str__(self):
         return f"log_plan_item('{self.message}')"
 
+    def __repr__(self):
+        return str(self)
+
 
 class GetDonePlanItem(PlanItemWithSemanticContent):
     def __init__(self, action):
         PlanItemWithSemanticContent.__init__(self, PlanItem.TYPE_GET_DONE, action)
```

## tala/model/proposition.py

```diff
@@ -52,14 +52,17 @@
     def __eq__(self, other):
         try:
             return other.is_proposition() and self.get_type() == other.get_type() and self.get_polarity(
             ) == other.get_polarity()
         except AttributeError:
             return False
 
+    def __hash__(self):
+        return hash((self.get_type(), self.get_polarity()))
+
     def get_polarity_prefix_string(self):
         if self._polarity == Polarity.NEG:
             return "~"
         else:
             return ""
 
     def get_type(self):
@@ -499,21 +502,26 @@
         self.parameters = parameters
         Proposition.__init__(self, Proposition.SERVICE_ACTION_STARTED)
         OntologySpecificSemanticObject.__init__(self, ontology_name)
 
     def __eq__(self, other):
         try:
             return (
-                other.is_proposition() and other.is_service_action_started_proposition()
-                and other.ontology_name == self.ontology_name and other.service_action == self.service_action
+                other.is_proposition()
+                and other.is_service_action_started_proposition()
+                and other.ontology_name == self.ontology_name
+                and other.service_action == self.service_action
                 and other.get_polarity() == self.get_polarity()
             )
         except AttributeError:
             return False
 
+    def __hash__(self):
+        return hash((self.ontology_name, self.service_action, self.get_polarity()))
+
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __str__(self):
         return "ServiceActionStartedProposition(%s, %s)" % (self.service_action, unicodify(self.parameters))
 
 
@@ -741,15 +749,15 @@
         except AttributeError:
             return False
 
     def __str__(self):
         return f"action_status({self.content}, {self.status})"
 
     def __hash__(self):
-        return hash(self.content, self.status)
+        return hash((self.content, self.status))
 
 
 class ImplicationProposition(PropositionWithSemanticContent):
     def __init__(self, antecedent, consequent):
         self._antecedent = antecedent
         self._consequent = consequent
         PropositionWithSemanticContent.__init__(self, Proposition.IMPLICATION, (antecedent, consequent))
```

## tala/nl/abstract_generator.py

```diff
@@ -1,14 +1,14 @@
 import os
 
 from tala.ddd.grammar.reader import GrammarReader
 from tala.model.grammar.intent import Answer, AnswerNegation
 from tala.model.grammar.required_entity import RequiredSortalEntity
 from tala.nl.examples import Examples
-from tala.nl.generated_intent import GeneratedIntent
+from tala.nl.generated_intent import GeneratedCustomIntent
 from tala.nl.constants import ANSWER_INTENT, ANSWER_NEGATION_INTENT
 
 
 class GrammarFormatNotSupportedException(Exception):
     pass
 
 
@@ -73,15 +73,15 @@
         def samples(requests):
             for request in requests:
                 for sample in self._create_intent_samples(grammar, ddd, request):
                     yield sample
 
         intent = self._format_action(action)
         requests = list(grammar.requests_of_action(action))
-        return GeneratedIntent(intent, requests, list(samples(requests)))
+        return GeneratedCustomIntent(intent, requests, list(samples(requests)))
 
     def _examples_of_questions(self, grammar, ddd):
         for resolve_goal in self._ddd.domain.get_all_resolve_goals():
             question = resolve_goal.get_question()
             yield self._generated_question_intent_for(grammar, ddd, question)
 
     def _generated_question_intent_for(self, grammar, ddd, question):
@@ -89,15 +89,15 @@
             for question in questions:
                 for sample in self._create_intent_samples(grammar, ddd, question):
                     yield sample
 
         predicate = question.get_predicate().get_name()
         intent = self._format_question(predicate)
         questions = list(grammar.questions_of_predicate(predicate))
-        return GeneratedIntent(intent, questions, list(samples(questions)))
+        return GeneratedCustomIntent(intent, questions, list(samples(questions)))
 
     def _examples_of_answers(self, grammar, ddd):
         def samples_from_sorts(sorts):
             for sort in sorts:
                 templates = list(self._language_examples.answer_templates)
                 for sample in self._create_sortal_answer_samples(grammar, ddd, sort, templates):
                     yield sample
@@ -111,15 +111,15 @@
             for sort in sorts:
                 yield Answer(["", ""], [RequiredSortalEntity(sort.get_name())])
 
         sorts = self._ddd.ontology.predicate_sorts
         explicit_answers = list(grammar.answers())
         answers = list(answers_from_sorts(sorts)) + explicit_answers
         samples = list(samples_from_sorts(sorts)) + list(samples_from_explicit_answers(explicit_answers))
-        yield GeneratedIntent(ANSWER_INTENT, answers, samples)
+        yield GeneratedCustomIntent(ANSWER_INTENT, answers, samples)
 
     def _examples_of_answer_negations(self, grammar, ddd):
         def generate_samples(sorts):
             for sort in sorts:
                 templates = list(self._language_examples.answer_negation_templates)
                 for sample in self._create_sortal_answer_samples(grammar, ddd, sort, templates):
                     yield sample
@@ -127,15 +127,15 @@
         def answers_from_sorts(sorts):
             for sort in sorts:
                 yield AnswerNegation(["", ""], [RequiredSortalEntity(sort.get_name())])
 
         sorts = [sort for sort in self._ddd.ontology.predicate_sorts if not sort.is_string_sort()]
         answers = list(answers_from_sorts(sorts))
         samples = list(generate_samples(sorts))
-        yield GeneratedIntent(ANSWER_NEGATION_INTENT, answers, samples)
+        yield GeneratedCustomIntent(ANSWER_NEGATION_INTENT, answers, samples)
 
     def _all_individual_grammar_entries_of_custom_sort(self, grammar, sort):
         individuals = self._ddd.ontology.get_individuals_of_sort(sort.get_name())
         for individual in individuals:
             yield grammar.entries_of_individual(individual)
 
     def _all_individuals_of_custom_sort(self, grammar, sort):
```

## tala/nl/examples.py

```diff
@@ -43,14 +43,22 @@
         raise NotImplementedError()
 
     @property
     def up(self):
         raise NotImplementedError()
 
     @property
+    def done(self):
+        raise NotImplementedError()
+
+    @property
+    def negative_perception(self):
+        raise NotImplementedError()
+
+    @property
     def answer_templates(self):
         yield Template('{{ name }}')
 
     @property
     def answer_negation_templates(self):
         raise NotImplementedError()
 
@@ -65,15 +73,20 @@
             return self.datetime
         if sort.is_person_name_sort():
             return self.person_name
         raise SortNotSupportedException("Builtin sort '%s' is not yet supported together with RASA" % sort.get_name())
 
     @staticmethod
     def from_language(language_code):
-        examples = {ENGLISH: EnglishExamples(), SWEDISH: SwedishExamples(), SPANISH: SpanishExamples(), PERSIAN: PersianExamples()}
+        examples = {
+            ENGLISH: EnglishExamples(),
+            SWEDISH: SwedishExamples(),
+            SPANISH: SpanishExamples(),
+            PERSIAN: PersianExamples()
+        }
         return examples[language_code]
 
 
 class EnglishExamples(Examples):
     @property
     def negative(self):
         phrases = [
@@ -154,34 +167,56 @@
     @property
     def up(self):
         return [
             "go back", "back", "previous", "back to the previous", "go to the previous", "go back to the previous one"
         ]
 
     @property
+    def done(self):
+        return [
+            "I'm done", "done", "ready", "it's ready", "I'm ready", "completed", "check", "I have finished", "finished",
+            "done and done", "it's done now", "okay next", "next", "next instruction"
+        ]
+
+    @property
+    def negative_perception(self):
+        return [
+            "repeat",
+            "repeat it",
+            "repeat that",
+            "pardon",
+            "sorry",
+            "can you repeat that",
+            "excuse me",
+            "what was that",
+            "what did you say",
+            "come again",
+        ]
+
+    @property
     def answer_negation_templates(self):
         yield Template('not {{ name }}')
 
 
 class SwedishExamples(Examples):
     @property
     def negative(self):
         phrases = [
             "om", "ovanför", "tvärsöver", "efter", "mot", "bland", "runt", "som", "på", "vid", "ovanpå", "före",
             "bakom", "nedan", "under", "bredvid", "mellan", "bortom", "men", "av", "trots", "ner", "förutom", "för",
-            "från", "i", "inuti", "in i", "nära", "nästa", "mittemot", "ut", "utanför", "över", "per", "plus",
-            "runt", "sedan", "än", "genom", "tills", "till", "mot", "olik", "upp", "via", "med", "inom", "utan", "är",
-            "vara", "den", "det", "en", "ett", "dem", "denna", "detta", "jag", "du", "ni", "han", "hon", "hen", "de",
-            "hans", "hennes", "hens", "min", "mina", "deras", "er", "din", "vi", "oss", "vår"
+            "från", "i", "inuti", "in i", "nära", "nästa", "mittemot", "ut", "utanför", "över", "per", "plus", "runt",
+            "sedan", "än", "genom", "tills", "till", "mot", "olik", "upp", "via", "med", "inom", "utan", "är", "vara",
+            "den", "det", "en", "ett", "dem", "denna", "detta", "jag", "du", "ni", "han", "hon", "hen", "de", "hans",
+            "hennes", "hens", "min", "mina", "deras", "er", "din", "vi", "oss", "vår"
         ]
         question_phrases = ["hur", "hur är", "när", "när är", "vad", "vad är", "varför", "varför är"]
         action_phrases = [
             "gör", "göra", "skapa", "berätta", "tala om", "börja", "starta", "sluta", "stopp", "stanna", "sätt på",
-            "stäng av", "höj", "sänk", "öka", "minska", "agera", "bestäm", "säg", "fråga", "gå", "kör",
-            "vänta", "ok", "visa", "hjälp"
+            "stäng av", "höj", "sänk", "öka", "minska", "agera", "bestäm", "säg", "fråga", "gå", "kör", "vänta", "ok",
+            "visa", "hjälp"
         ]
         for phrase in phrases:
             yield phrase
         for phrase in question_phrases:
             yield phrase
         for phrase in action_phrases:
             yield phrase
@@ -190,17 +225,16 @@
     def integer(self):
         return ["0", "99", "1224", "etthundratjugosju", "tre", "tvåtusenfemton"]
 
     @property
     def string(self):
         return [
             "enkel", "dubbelt ord", "det blir tre", "fyra på en gång", "ju fler desto bättre fem",
-            "håll andan och räkna till sex", "led dem fram till de glada sju",
-            "ingen räknar tår som den med åtta tår", "det spelar roll att det låter rimligt för nio",
-            "tar du med tio eller inga till en öde ö"
+            "håll andan och räkna till sex", "led dem fram till de glada sju", "ingen räknar tår som den med åtta tår",
+            "det spelar roll att det låter rimligt för nio", "tar du med tio eller inga till en öde ö"
         ]
 
     @property
     def datetime(self):
         return [
             "idag", "måndag 18 mars", "1:a mars", "klockan 11.45", "följande tre veckor", "om tio minuter",
             "20:e mars vid 22.00", "tjugonde mars vid tio på kvällen"
@@ -233,16 +267,36 @@
 
     @property
     def top(self):
         return ["glöm alltihop", "jag skiter i detta", "ta mig härifrån", "börja om", "börja från noll"]
 
     @property
     def up(self):
+        return ["gå tillbaka", "vad var den förra", "backa", "förra", "tillbaka", "ta mig tillbaka", "backa till förra"]
+
+    @property
+    def done(self):
         return [
-            "gå tillbaka", "vad var den förra", "backa", "förra", "tillbaka", "ta mig tillbaka", "backa till förra"
+            "jag är klar", "klar", "färdig", "nu är det gjort", "jag har gjort klart", "slutfört", "det var det",
+            "nu är det klart", "det är färdigt", "okej nästa", "nästa", "nästa instruktion", "jag är färdig"
+        ]
+
+    @property
+    def negative_perception(self):
+        return [
+            "ursäkta",
+            "förlåt",
+            "kan du repetera det",
+            "repetera",
+            "repetera det",
+            "upprepa",
+            "upprepa vad du sa",
+            "vad sa du",
+            "ta det en gång till",
+            "va",
         ]
 
     @property
     def answer_negation_templates(self):
         yield Template('inte {{ name }}')
 
 
@@ -253,28 +307,28 @@
             "a bordo", "acerca de", "arriba", "a través de", "después de", "en contra", "a lo largo de", "entre",
             "como", "en", "en", "en lo alto", "antes", "detrás", "abajo", "debajo", "al lado", "entre", "más allá de",
             "pero", "por", "abajo", "durante", "excepto", "para", "desde", "en", "dentro", "en", "menos", "como",
             "cerca", "de", "encima de", "sobre", "opuesto", "fuera", "fuera de", "corto", "desde", "que", "entonces",
             "a lo largo de", "hasta", "hacia", "debajo de", "a diferencia de", "hasta", "arriba", "con", "dentro de",
             "sin", "vale", "es"
             "se", "el", "la"
-            "a", "soy", "son", "ellos", "este", "ese", "yo", "usted ", "él", "ella", "ellos", "ellas", "su", "sus",
-            "mi", "tu", "tú", "nosotros", "nosotras", "vosotros", "vosotras", "nuestro", "nuestra", "vuestro",
-            "vuestra", "vuestros", "vuestras", "mío", "mía", "míos", "mías", "tuyo", "tuyos", "tuya", "tuyas",
-            "suyo", "suya", "suyos", "suyas"
+            "a", "soy", "son", "ellos", "este", "ese", "yo", "usted", "él", "ella", "ellos", "ellas", "su", "sus", "mi",
+            "tu", "tú", "nosotros", "nosotras", "vosotros", "vosotras", "nuestro", "nuestra", "vuestro", "vuestra",
+            "vuestros", "vuestras", "mío", "mía", "míos", "mías", "tuyo", "tuyos", "tuya", "tuyas", "suyo", "suya",
+            "suyos", "suyas"
         ]
         question_phrases = [
             "cómo", "cómo está", "cómo es", "cómo está el", "cómo es el", "cómo está la", "cómo es la",
             "cómo están los", "cómo están las"
-            "cuándo", "cuándo es", "cuándo está", "cuándo es el", "cuándo es la", "cuándo son los",
-            "cuándo son las", "cuándo está el", "cuándo está la", "cuándo están los", "cuándo están las", "qué",
-            "qué es", "qué es la", "qué es el", "qué son los", "qué son las", "cuál", "cuál es", "cuál es la",
-            "cuál es el", "cuáles son los", "cuáles son las", "por qué", "por qué es", "por qué está",
-            "por qué es el", "por qué es la", "por qué son", "por qué son los", "por qué son las",
-            "por qué está el", "por qué está la", "por qué están los", "por qué están las"
+            "cuándo", "cuándo es", "cuándo está", "cuándo es el", "cuándo es la", "cuándo son los", "cuándo son las",
+            "cuándo está el", "cuándo está la", "cuándo están los", "cuándo están las", "qué", "qué es", "qué es la",
+            "qué es el", "qué son los", "qué son las", "cuál", "cuál es", "cuál es la", "cuál es el", "cuáles son los",
+            "cuáles son las", "por qué", "por qué es", "por qué está", "por qué es el", "por qué es la", "por qué son",
+            "por qué son los", "por qué son las", "por qué está el", "por qué está la", "por qué están los",
+            "por qué están las"
         ]
         action_phrases = [
             "hacer", "decir", "iniciar", "detener", "habilitar", "deshabilitar", "querer", "dar", "haber"
             "subir", "bajar", "disminuir", "aumentar", "actuar", "determinar", "preguntar", "ir", "disparar", "esperar",
             "esperar", "aceptar", "mostrar", "enseñar", "ayudar"
         ]
         for phrase in phrases:
@@ -283,16 +337,16 @@
             yield phrase
         for phrase in action_phrases:
             yield phrase
 
     @property
     def integer(self):
         return [
-            "0", "99", "1224", "100000", "100.000", "una", "uno", "dieciséis", "veintiuno", "veintiuno",
-            "veinte y uno", "tres", "dos mil quince", "mil cincuenta y siete"
+            "0", "99", "1224", "100000", "100.000", "una", "uno", "dieciséis", "veintiuno", "veintiuno", "veinte y uno",
+            "tres", "dos mil quince", "mil cincuenta y siete"
         ]
 
     @property
     def string(self):
         return [
             "singular", "doble palabra", "tres en uno", "hey pon cuatro", "cuanto más mejor cinco",
             "cálmate y cuenta hasta seis", "llévalos hasta el siete",
@@ -308,28 +362,27 @@
             "próximos tres meses", "este fin de semana", "el 12 de marzo a las 8 de la mañana"
         ]
 
     @property
     def person_name(self):
         return [
             "Antonio", "José", "Manuel", "Francisco", "David", "Juan", "Javier", "Daniel", "Jesús", "Carlos",
-            "Alejandro", "Miguel", "Pedro", "Pablo", "Ángel", "Sergio", "Alberto", "María", "Cármen", "Ana",
-            "Isabel", "Laura", "Cristina", "Marta", "Dolores", "Lucía", "Paula", "Mercedes", "Rosario", "Teresa",
-            "Sara", "Reyes", "Caballero", "Nieto", "Pascual", "Ferrer", "Giménez", "Lorenzo", "Pastor", "Soto",
-            "Soler", "Parra", "García", "González", "López", "Pérez", "Gómez", "Díaz", "Alonso", "Moreno",
-            "Navarro", "Rámos", "Torres", "Castillo", "Carlos Aguilar Moreno", "Pedro Sánchez Álvarez",
-            "Sonia Reina Sanz", "Cristina Claret Iglesias", "Manuel Núñez Santos", "Rafael Rubio Molina",
-            "Isabel Tomás Comas", "Anna Delgado Prieto", "Lorena Fuentes Ortiz", "Silvia Carrasco Rojas"
+            "Alejandro", "Miguel", "Pedro", "Pablo", "Ángel", "Sergio", "Alberto", "María", "Cármen", "Ana", "Isabel",
+            "Laura", "Cristina", "Marta", "Dolores", "Lucía", "Paula", "Mercedes", "Rosario", "Teresa", "Sara", "Reyes",
+            "Caballero", "Nieto", "Pascual", "Ferrer", "Giménez", "Lorenzo", "Pastor", "Soto", "Soler", "Parra",
+            "García", "González", "López", "Pérez", "Gómez", "Díaz", "Alonso", "Moreno", "Navarro", "Rámos", "Torres",
+            "Castillo", "Carlos Aguilar Moreno", "Pedro Sánchez Álvarez", "Sonia Reina Sanz",
+            "Cristina Claret Iglesias", "Manuel Núñez Santos", "Rafael Rubio Molina", "Isabel Tomás Comas",
+            "Anna Delgado Prieto", "Lorena Fuentes Ortiz", "Silvia Carrasco Rojas"
         ]
 
     @property
     def yes(self):
         return [
-            "sí", "claro", "desde luego", "por supuesto", "de acuerdo", "vale", "perfecto", "bien", "okei", "sip",
-            "sep"
+            "sí", "claro", "desde luego", "por supuesto", "de acuerdo", "vale", "perfecto", "bien", "okei", "sip", "sep"
         ]
 
     @property
     def no(self):
         return ["no", "de ningún modo", "de ninguna manera", "en absoluto", "na", "nop", "ni de broma", "para nada"]
 
     @property
@@ -338,37 +391,57 @@
             "vuelve a empezar", "vuelve al principio", "vuelve al inicio", "principio", "inicio", "desde el principio",
             "reinicia", "empieza de nuevo", "olvídalo", "olvida todo"
         ]
 
     @property
     def up(self):
         return [
-            "atrás", "vuelve atrás", "vuelve", "regresa", "vuelve una atrás", "quiero ir atrás",
-            "quiero volver atrás"
+            "atrás", "vuelve atrás", "vuelve", "regresa", "vuelve una atrás", "quiero ir atrás", "quiero volver atrás"
+        ]
+
+    @property
+    def done(self):
+        return [
+            "Ya está", "listo", "completado", "hecho", "ya he acabado", "acabado", "ya está listo", "ya estoy",
+            "ya está hecho"
+        ]
+
+    @property
+    def negative_perception(self):
+        return [
+            "repite",
+            "puedes repetir",
+            "repite por favor",
+            "otra vez",
+            "dilo otra vez",
+            "qué",
+            "cómo",
+            "cómo has dicho",
+            "qué has dicho",
         ]
 
     @property
     def answer_negation_templates(self):
         yield Template('no {{ name }}')
 
 
 class PersianExamples(Examples):
     @property
     def negative(self):
         phrases = [
             "داخل", "درباره", "بالا", "در سراسر", "بعد", "علیه", "همراه", "در بین", "به عنوان", "در", "روی", "بالای",
-            "قبل", "پشت", "زیر", "زیر", "کنار", "بین", "فراتر", "اما", "توسط", "بیا", "پایین", "هنگام", "به جز",
-            "برای", "از", "در", "داخل", "به", "کمتر", "مانند", "نزدیک", "از", "خاموش", "روشن", "روی", "مخالف",
-            "خارج", "بیش", "گذشته", "ذخیره", "کوتاه", "از", "بعد", "از طریق", "سراسر", "به", "به سمت", "زیر",
-            "بر خلاف", "تا", "بالا", "بر", "با", "بدون", "ارزش", "است", "آن", "این", "یک", "من", "هستند", "آنها",
-            "این", "آن", "من", "شما", "او", "آنها", "ایشان", "او", "اون", "مال", "آنها", "شما", "ما"
+            "قبل", "پشت", "زیر", "زیر", "کنار", "بین", "فراتر", "اما", "توسط", "بیا", "پایین", "هنگام", "به جز", "برای",
+            "از", "در", "داخل", "به", "کمتر", "مانند", "نزدیک", "از", "خاموش", "روشن", "روی", "مخالف", "خارج", "بیش",
+            "گذشته", "ذخیره", "کوتاه", "از", "بعد", "از طریق", "سراسر", "به", "به سمت", "زیر", "بر خلاف", "تا", "بالا",
+            "بر", "با", "بدون", "ارزش", "است", "آن", "این", "یک", "من", "هستند", "آنها", "این", "آن", "من", "شما", "او",
+            "آنها", "ایشان", "او", "اون", "مال", "آنها", "شما", "ما"
         ]
         question_phrases = [
-            "چگونه", "چطور", "چه وقت", "چه وقتی", "برای چه", "وقتی", "چه زمانی", "چه موقع", "کی" "چه زمانی", "چه",
-            "برای چی", "چطور میشه که", "چی میشه که", "برای چه", "چرا"
+            "چگونه", "چطور", "چه وقت", "چه وقتی", "برای چه", "وقتی", "چه زمانی", "چه موقع", "کی"
+            "چه زمانی", "چه", "برای چی", "چطور میشه که", "چی میشه که", "برای چه", "چرا"
         ]
         action_phrases = [
             "انجام بده", "بساز", "بگو", "شروع کن", "متوقف کن", "فعال کن", "غیرفعال کن", "افزایش بده", "پایین بیار",
             "کاهش بده", "افزایش بده", "عمل کن", "تعیین کن", "بگو", "سؤال کن", "برو", "شلیک کن", "صبر کن", "متوقف شو",
             "نشون بده", "نمایش بده", "کمک کن"
         ]
         for phrase in phrases:
@@ -382,55 +455,77 @@
     def integer(self):
         return ["0", "99", "1224", "صد و پنجاه و هفت", "سه", "دو هزار و پانزده"]
 
     @property
     def string(self):
         return [
             "تک", "کلمه دوتایی", "سه در یک", "چهار تاش  از اونها بده", "پنج انگشت با هم برابرند",
-            "آرام باش و تا شش بشمر", "توی هفت آسمون یک ستاره هم نداره",
-            "هیچکس انگشتها رو مثل آن هشت انگشتی نمیشناسد",
-            "مهم هست که برای ما نه نفر معنی داره",
-            "لطفا ده تا یا هیچ کدام را به جزیره بیاورید"
+            "آرام باش و تا شش بشمر", "توی هفت آسمون یک ستاره هم نداره", "هیچکس انگشتها رو مثل آن هشت انگشتی نمیشناسد",
+            "مهم هست که برای ما نه نفر معنی داره", "لطفا ده تا یا هیچ کدام را به جزیره بیاورید"
         ]
 
     @property
     def datetime(self):
         return [
-            "امروز", "دوشنبه ۱۸ مارش", "اول مارش", "11:45 صبح", "سه هفته بعد", "ده دقیقه بعد",
-            "20 مارش ساعت 22:00", "بیستم مارش ساعت 10 صبح"
+            "امروز", "دوشنبه ۱۸ مارش", "اول مارش", "11:45 صبح", "سه هفته بعد", "ده دقیقه بعد", "20 مارش ساعت 22:00",
+            "بیستم مارش ساعت 10 صبح"
         ]
 
     @property
     def person_name(self):
         return [
-            "علی", "فاطمه", "آرمان", "شیوا", "فرناز", "آریا", "رویا",
-            "فرناز عطایی", "سعید صادقپور", "حامد زاهدی", "آرمان بحری"
+            "علی", "فاطمه", "آرمان", "شیوا", "فرناز", "آریا", "رویا", "فرناز عطایی", "سعید صادقپور", "حامد زاهدی",
+            "آرمان بحری"
         ]
 
     @property
     def yes(self):
         return [
-            "بله", "آره", "مطمئن", "مطمئنم", "اوکی", "البته", "خیلی خوب", "خوبه", "درست", "درسته", "عالی",
-            "عالیه", "من اینطور فکر میکنم"
+            "بله", "آره", "مطمئن", "مطمئنم", "اوکی", "البته", "خیلی خوب", "خوبه", "درست", "درسته", "عالی", "عالیه",
+            "من اینطور فکر میکنم"
         ]
 
     @property
     def no(self):
-        return [
-            "نه", "نه متشکرم", "نه ممنون", "نه خیلی ممنون", "منفی", "اینو نمیخوام", "نیمخوام", "نکن", "لطفا نکن"
-        ]
+        return ["نه", "نه متشکرم", "نه ممنون", "نه خیلی ممنون", "منفی", "اینو نمیخوام", "نیمخوام", "نکن", "لطفا نکن"]
 
     @property
     def top(self):
         return [
             "فراموش کن", "ولش کن", "منو از اینجا بیرون ببر", "دوباره شورع کن", "ابتدا", "اینو ولش کن", "شروع دوباره"
         ]
 
     @property
     def up(self):
+        return ["برو عقب", "عقب", "قبلی", "برو به عقب", "برو به قبلی", "قبلیه"]
+
+    @property
+    def done(self):
         return [
-            "برو عقب", "عقب", "قبلی", "برو به عقب", "برو به قبلی", "قبلیه"
+            "من تمام شدم",
+            "انجام شده",
+            "تکمیل شده",
+            "بررسی",
+            "من تمام کرده ام",
+            "تمام شده",
+            "انجام شده و انجام شده",
+            "الان تمام شده",
+        ]
+
+    @property
+    def negative_perception(self):
+        return [
+            "تکرار",
+            "تکرار کن",
+            "تکرار کنید",
+            "بخشش",
+            "متاسف",
+            "آیا می توانید آن را تکرار کنید؟",
+            "ببخشید",
+            "آن چه بود",
+            "چی گفتی",
+            "دوباره بیا",
         ]
 
     @property
     def answer_negation_templates(self):
         yield Template('not {{ name }}')
```

## tala/nl/generated_intent.py

```diff
@@ -1,15 +1,49 @@
-from collections import namedtuple, OrderedDict
+from collections import OrderedDict
 from itertools import chain
 
+from tala.utils.equality import EqualityMixin
+
+
+class GeneratedIntent(EqualityMixin):
+    def __init__(self, name, samples):
+        self._name = name
+        self._samples = samples
+
+    @property
+    def name(self):
+        return self._name
+
+    @property
+    def samples(self):
+        return self._samples
+
+
+class GeneratedBuiltinRequestIntent(GeneratedIntent):
+    @property
+    def name(self):
+        return f"request:{self._name}"
+
+
+class GeneratedBuiltinReportIntent(GeneratedIntent):
+    @property
+    def name(self):
+        return f"report:{self._name}"
+
+
+class GeneratedBuiltinAnswerIntent(GeneratedIntent):
+    @property
+    def name(self):
+        return f"answer:{self._name}"
+
+
+class GeneratedCustomIntent(GeneratedIntent):
+    def __init__(self, name, sources, samples):
+        super().__init__(name, samples)
+        self._sources = sources
 
-class GeneratedIntent(namedtuple("GeneratedIntent", ["name", "sources", "samples"])):
     @property
     def required_entities(self):
-        lists = [source.required_entities for source in self.sources]
+        lists = [source.required_entities for source in self._sources]
         all_entities = chain(*lists)
         unique_entities = list(OrderedDict.fromkeys(all_entities))
         return unique_entities
-
-
-class GeneratedBuiltinIntent(namedtuple("GeneratedBuiltinIntent", ["name", "samples"])):
-    pass
```

## tala/nl/rasa/generator.py

```diff
@@ -1,21 +1,26 @@
 from io import StringIO
 import warnings
 
 from jinja2 import Template
 
 from tala.model.action import TOP, UP
+from tala.model.action_status import DONE
 from tala.model.individual import Yes, No
+from tala.model.move import ICMMove
 from tala.model.sort import STRING
 from tala.nl.abstract_generator import AbstractGenerator, UnexpectedPropositionalEntityEncounteredException, \
     UnexpectedRequiredEntityException
 from tala.nl.constants import ACTION_INTENT, QUESTION_INTENT, NEGATIVE_INTENT
-from tala.nl.generated_intent import GeneratedBuiltinIntent
+from tala.nl.generated_intent import GeneratedIntent, GeneratedBuiltinAnswerIntent, GeneratedBuiltinRequestIntent, \
+    GeneratedBuiltinReportIntent
 from tala.nl import languages
 
+NEGATIVE_PERCEPTION_ICM = ICMMove(ICMMove.PER, polarity=ICMMove.NEG)
+
 
 class RasaGenerator(AbstractGenerator):
     @property
     def _language(self):
         return languages.RASA_LANGUAGE[self._language_code]
 
     def stream(self, file_object):
@@ -90,19 +95,23 @@
             synonym_objects=synonyms,
             ddd=self._ddd.name
         )
 
         return rasa_data
 
     def _general_examples(self):
-        yield GeneratedBuiltinIntent(NEGATIVE_INTENT, list(self._language_examples.negative))
-        yield GeneratedBuiltinIntent(Yes.YES, self._language_examples.yes)
-        yield GeneratedBuiltinIntent(No.NO, self._language_examples.no)
-        yield GeneratedBuiltinIntent(TOP, self._language_examples.top)
-        yield GeneratedBuiltinIntent(UP, self._language_examples.up)
+        yield GeneratedIntent(NEGATIVE_INTENT, list(self._language_examples.negative))
+        yield GeneratedBuiltinAnswerIntent(Yes.YES, self._language_examples.yes)
+        yield GeneratedBuiltinAnswerIntent(No.NO, self._language_examples.no)
+        yield GeneratedBuiltinRequestIntent(TOP, self._language_examples.top)
+        yield GeneratedBuiltinRequestIntent(UP, self._language_examples.up)
+        yield GeneratedBuiltinReportIntent(DONE, self._language_examples.done)
+        yield GeneratedIntent(
+            NEGATIVE_PERCEPTION_ICM.as_semantic_expression(), self._language_examples.negative_perception
+        )
 
     def _entity_synonyms_from_custom_sorts(self, grammar):
         for sort in list(self._ddd.ontology.get_sorts().values()):
             if sort.is_builtin():
                 continue
             for individual, grammar_entries in self._all_individuals_of_custom_sort(grammar, sort):
                 if len(grammar_entries) <= 1:
```

## tala/testing/interactions/compiler.py

```diff
@@ -1,26 +1,28 @@
+import contextlib
 import re
 import json
 
 from tala.testing.interactions.named_test import InteractionTest
 from tala.testing.interactions.turn import UserPassivityTurn, UserInterpretationTurn, SystemUtteranceTurn, \
-    RecognitionHypothesesTurn, NotifyStartedTurn, SystemMovesTurn
+    RecognitionHypothesesTurn, NotifyStartedTurn, SystemMovesTurn, UserSemanticInputTurn
 from tala.model.event_notification import EventNotification
 
 
 class ParseException(Exception):
     pass
 
 
 class InteractionTestCompiler(object):
     VALID_TURN_TYPES = ["U>", "S>", "Event>"]
 
     _turn_matcher = re.compile('^(%s) ?(.*)$' % "|".join(VALID_TURN_TYPES), re.MULTILINE | re.DOTALL)
     _moves_matcher = re.compile(r'([\[{].*[\]}])$')
-    _utterance_string_and_confidence_matcher = re.compile(r'(.+) (\$\w+|\d*\.\d+)?$')
+    _utterance_matcher = re.compile(r'^([\'"]?)(?P<utterance>.*)\1$')
+    _confidence_matcher = re.compile(r'^.*\s+(?P<confidence>\$\w+|\d*\.\d+)$')
     _hypothesis_split_re = re.compile(r'\s*\|\s*')
 
     def compile_interaction_tests(self, filename, file_):
         self._filename = filename
         self._file = file_
         self._result = []
         self._line_number = 0
@@ -111,17 +113,26 @@
         else:
             raise ParseException(
                 "Expected one of %s on line %d in '%s' but got '%s'." %
                 (self.VALID_TURN_TYPES, self._line_number, self._filename, turn_content_as_string)
             )
 
     def _parse_user_input_turn(self, turn_content_as_string):
+        def is_semantic_input():
+            with self._json_guard(turn_content_as_string):
+                content = json.loads(turn_content_as_string)
+            if isinstance(content, dict):
+                return "interpretations" in turn_content_as_string
+            return False
+
         if not turn_content_as_string:
             return UserPassivityTurn(self._line_number)
         if self._is_moves_content_string(turn_content_as_string):
+            if is_semantic_input():
+                return UserSemanticInputTurn(json.loads(turn_content_as_string), self._line_number)
             moves, utterance, modality = self._parse_moves_content_string(turn_content_as_string)
             return UserInterpretationTurn(moves, self._line_number, utterance=utterance, modality=modality)
         hypothesis_list = self._get_hypothesis_list(turn_content_as_string)
         return RecognitionHypothesesTurn(hypothesis_list, self._line_number)
 
     def _parse_system_output_turn(self, turn_content_as_string):
         if self._is_moves_content_string(turn_content_as_string):
@@ -155,32 +166,45 @@
         m = self._moves_matcher.search(string)
         if not m:
             raise ParseException(
                 "Expected a list of moves or an interpretation object on line %d in '%s' but got '%s'." %
                 (self._line_number, self._filename, string)
             )
         (string, ) = m.groups()
-        try:
+        with self._json_guard(string):
             json_value = json.loads(string)
+        return extract(json_value)
+
+    @contextlib.contextmanager
+    def _json_guard(self, string):
+        try:
+            yield
         except json.decoder.JSONDecodeError as exception:
             raise ParseException(
                 f"Expected valid JSON on line {self._line_number} of '{self._filename}' "
                 f"but encountered a decoding error.\n\n"
                 f"  Line {self._line_number}: {string}\n\n"
                 f"  Error: '{exception}'"
             )
-        return extract(json_value)
 
-    def _parse_hypothesis_as_string(self, unicode_string):
-        m = self._utterance_string_and_confidence_matcher.search(unicode_string)
-        if m:
-            (utterance_string_unicode, confidence) = m.groups()
-            return (utterance_string_unicode, confidence)
-        else:
-            return (unicode_string, None)
+    def _parse_hypothesis_as_string(self, string):
+        def confidence():
+            match = self._confidence_matcher.search(string)
+            return match.group("confidence") if match else None
+
+        def strip_confidence():
+            confidence_part = confidence()
+            return string.replace(confidence_part, "").strip() if confidence_part else string
+
+        def utterance():
+            utterance_part = strip_confidence()
+            match = self._utterance_matcher.search(utterance_part)
+            return match.group("utterance")
+
+        return utterance(), confidence()
 
     def _parse_event_turn(self, string):
         try:
             json_dict = json.loads(string)
         except Exception as json_exception:
             raise ParseException(
                 "Expected a JSON parseable string on line %d in '%s' but got '%s'. JSON exception: %s" %
@@ -194,22 +218,44 @@
             )
 
     @classmethod
     def pretty_passivity(cls):
         return "U>"
 
     @classmethod
+    def pretty_interpretation(cls, interpretation):
+        return f"U> {json.dumps(interpretation)}"
+
+    @classmethod
+    def pretty_semantic_input(cls, request):
+        return f"U> {json.dumps(request)}"
+
+    @classmethod
+    def pretty_semantic_expressions(cls, semantic_expressions):
+        return f"U> {json.dumps(semantic_expressions)}"
+
+    @classmethod
+    def pretty_event(cls, event_dictionary):
+        return f"Event> {json.dumps(event_dictionary)}"
+
+    @classmethod
     def pretty_system_utterance(cls, utterance):
-        return "S> %s" % utterance
+        return f"S> {utterance}"
 
     @classmethod
-    def pretty_hypotheses(cls, hypotheses):
-        hypothesis_strings = [cls._pretty_hypothesis(hypothesis) for hypothesis in hypotheses]
-        utterances_with_confidence = " | ".join(hypothesis_strings)
-        return "U> %s" % utterances_with_confidence
+    def pretty_system_moves(cls, moves):
+        return f"S> {json.dumps(moves)}"
 
     @classmethod
-    def _pretty_hypothesis(cls, hypothesis):
-        utterance, confidence = hypothesis
-        if confidence == 1.0:
-            return utterance
-        return "%s %s" % (utterance, confidence)
+    def pretty_hypotheses(cls, hypotheses):
+        def pretty_utterance(utterance):
+            return utterance or "''"
+
+        def pretty_hypothesis(utterance, confidence):
+            utterance = pretty_utterance(utterance)
+            if str(confidence) == "1.0":
+                return utterance
+            return f"{utterance} {confidence}"
+
+        hypothesis_strings = [pretty_hypothesis(utterance, confidence) for utterance, confidence in hypotheses]
+        utterances_with_confidence = " | ".join(hypothesis_strings)
+        return f"U> {utterances_with_confidence}"
```

## tala/testing/interactions/testcase.py

```diff
@@ -1,11 +1,12 @@
 import fnmatch
 import json
 import re
 import unittest
+import warnings
 
 import structlog
 
 from tala.model.input_hypothesis import InputHypothesis
 from tala.model.event_notification import EventNotification
 from tala.utils.tdm_client import TDMClient, TDMRuntimeException
 from tala.model.user_move import UserMove  # noqa: F401
@@ -35,24 +36,38 @@
         self._logger = structlog.get_logger(__name__)
         self._tdm_client = TDMClient(environment_or_url)
 
         method_name = self._ensure_name_can_be_used_as_python_method(test.name)
         self._create_test_method(method_name)
         unittest.TestCase.__init__(self, method_name)
 
-        self._last_system_output_response = None
+        self.last_system_output_response = None
         self._detected_unexpected_passivity = False
 
     @property
+    def last_system_output_response(self):
+        return self._last_system_output_response
+
+    @last_system_output_response.setter
+    def last_system_output_response(self, new_response):
+        def check_for_warnings():
+            if new_response is not None and "warnings" in new_response and len(new_response["warnings"]) > 0:
+                for warning in new_response["warnings"]:
+                    warnings.warn(warning)
+
+        check_for_warnings()
+        self._last_system_output_response = new_response
+
+    @property
     def name(self):
         return self._test.name
 
     @property
     def session_id(self):
-        return self._last_system_output_response["session"]["session_id"]
+        return self.last_system_output_response["session"]["session_id"]
 
     @staticmethod
     def _ensure_name_can_be_used_as_python_method(name):
         return re.sub(r"\W", "_", name)
 
     def _create_test_method(self, name):
         setattr(self, name, self.perform)
@@ -77,15 +92,15 @@
             self._simulate_user_passivity(turn)
         elif turn.is_event_turn:
             self._handle_event_notification(turn)
         else:
             raise UnsupportedTurn("Expected one of the supported turns but got '%s'." % turn)
 
     def _start_session(self):
-        self._last_system_output_response = self._tdm_client.start_session()
+        self.last_system_output_response = self._tdm_client.start_session()
 
     def _handle_system_output_turn(self, turn):
         if turn.is_system_utterance_turn:
             self._expect_system_utterance(turn)
         elif turn.is_system_moves_turn:
             self._expect_system_moves(turn)
         else:
@@ -93,31 +108,45 @@
 
     def _simulate_user_input(self, turn):
         self._logger.debug("Simulating user input")
         if turn.is_recognition_hypotheses_turn:
             self._handle_recognition_hypotheses(turn)
         elif turn.is_user_interpretation_turn:
             self._handle_user_moves(turn)
+        elif turn.is_user_semantic_input_turn:
+            self._handle_user_interpretations(turn)
         else:
             raise UnsupportedTurn("Expected one of the supported user input turns but got '%s'." % turn)
 
     def _handle_recognition_hypotheses(self, turn):
-        self._last_system_output_response = self._send_natural_language_input_request(turn.hypotheses)
+        self.last_system_output_response = self._send_natural_language_input_request(turn.hypotheses)
 
     def _handle_user_moves(self, turn):
         def interpretation(moves, utterance, modality):
             if utterance:
                 modality = modality or Modality.SPEECH
                 return Interpretation(moves, modality, utterance=utterance)
             modality = modality or Modality.OTHER
             return InterpretationWithoutUtterance(moves, modality)
 
         moves = [self._create_move(move_as_string) for move_as_string in turn.moves]
         interpretations = [interpretation(moves, turn.utterance, turn.modality)]
-        self._last_system_output_response = self._tdm_client.request_semantic_input(self.session_id, interpretations)
+        self.last_system_output_response = self._tdm_client.request_semantic_input(self.session_id, interpretations)
+
+    def _handle_user_interpretations(self, turn):
+        body = {
+            "session": {
+                "session_id": self.session_id
+            },
+            "version": "3.3",
+            "request": {
+                "semantic_input": turn.semantic_input
+            }
+        }
+        self._last_system_output_response = self._tdm_client.make_request(body)
 
     def _create_move(self, move):
         def is_semantic_expression(move):
             return isinstance(move, str)
 
         def is_move_object(move):
             return isinstance(move, dict)
@@ -136,17 +165,17 @@
             semantic_expression,
             perception_confidence=perception_confidence,
             understanding_confidence=understanding_confidence
         )
 
     def _simulate_user_passivity(self, turn):
         self._logger.debug("Simulating user passivity")
-        if self._last_system_output_response and \
-           self._last_system_output_response["output"]["expected_passivity"] is not None:
-            self._last_system_output_response = self._tdm_client.request_passivity(self.session_id)
+        if self.last_system_output_response and \
+           self.last_system_output_response["output"]["expected_passivity"] is not None:
+            self.last_system_output_response = self._tdm_client.request_passivity(self.session_id)
         else:
             self._detected_unexpected_passivity = True
             self._line_number_of_unexpected_passivity = turn.line_number
 
     def _expect_system_utterance(self, system_utterance_turn):
         self._logger.debug("%s._expect_system_utterance(%s)" % (self.__class__.__name__, str(system_utterance_turn)))
         if self._detected_unexpected_passivity:
@@ -179,21 +208,20 @@
         )
 
     def _raise_and_log_assertion_error(self, error_string):
         self._logger.debug("Assertion error: %s" % error_string)
         raise AssertionError(error_string)
 
     def _get_system_utterance(self):
-        actual_utterance = self._last_system_output_response["output"]["utterance"]
+        actual_utterance = self.last_system_output_response["output"]["utterance"]
         self._logger.debug("Got system utterance %r" % actual_utterance)
-        self._last_system_output_response = self._last_system_output_response
         return actual_utterance
 
     def _get_system_moves(self):
-        actual_moves = self._last_system_output_response["output"]["moves"]
+        actual_moves = self.last_system_output_response["output"]["moves"]
         self._logger.debug(f"Got system moves {actual_moves!r}")
         return actual_moves
 
     def _assert_system_utterance_matches(self, pattern, utterance, line_number):
         if not fnmatch.fnmatch(utterance, pattern):
             self._fail_with_mismatch(line_number, pattern, utterance)
 
@@ -225,15 +253,15 @@
         explicit_score = m.group("explicit")
         if explicit_score:
             return float(explicit_score)
         raise InvalidConfidenceException("Invalid formatting of confidence: %s" % score)
 
     def _handle_event_notification(self, event_turn):
         if event_turn.is_notify_started_turn:
-            self._last_system_output_response = self._tdm_client.request_event_notification(
+            self.last_system_output_response = self._tdm_client.request_event_notification(
                 self.session_id, EventNotification(event_turn.action, EventNotification.STARTED, event_turn.parameters)
             )
         else:
             raise UnsupportedTurn("Expected one of the supported event turns but got '%s'." % event_turn)
 
 
 class StringComparison(object):
```

## tala/testing/interactions/turn.py

```diff
@@ -36,14 +36,18 @@
         return False
 
     @property
     def is_user_interpretation_turn(self):
         return False
 
     @property
+    def is_user_semantic_input_turn(self):
+        return False
+
+    @property
     def is_user_passivity_turn(self):
         return False
 
 
 class RecognitionHypothesesTurn(UserInputTurn):
     def __init__(self, hypotheses, line_number):
         super(RecognitionHypothesesTurn, self).__init__(line_number)
@@ -78,14 +82,28 @@
         return self._modality
 
     @property
     def utterance(self):
         return self._utterance
 
 
+class UserSemanticInputTurn(UserInputTurn):
+    def __init__(self, semantic_input, line_number):
+        super().__init__(line_number)
+        self._semantic_input = semantic_input
+
+    @property
+    def is_user_semantic_input_turn(self):
+        return True
+
+    @property
+    def semantic_input(self):
+        return self._semantic_input
+
+
 class UserPassivityTurn(Turn):
     @property
     def is_user_passivity_turn(self):
         return True
 
 
 class SystemOutputTurn(Turn):
```

## tala/utils/tdm_client.py

```diff
@@ -125,14 +125,17 @@
 
     def start_session(self, session_data: Mapping = None) -> Mapping:
         session_object = session_data or {}
         request = {"version": PROTOCOL_VERSION, "session": session_object, "request": {"start_session": {}}}
         response = self._make_request(request)
         return response
 
+    def make_request(self, *args, **kwargs):
+        return self._make_request(*args, **kwargs)
+
     def _make_request(self, request_body):
         data_as_json = json.dumps(request_body)
         headers = {'Content-type': 'application/json'}
         response_object = requests.post(self._url, data=data_as_json, headers=headers)
         response_object.raise_for_status()
         try:
             response = response_object.json()
```

## Comparing `tala-8.0.0.dist-info/METADATA` & `tala-9.0.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tala
-Version: 8.0.0
+Version: 9.0.0
 Summary: Design dialogue domain descriptions (DDDs) for TDM
 Home-page: http://www.talkamatic.se
 Author: Talkamatic
 Author-email: dev@talkamatic.se
 License: UNKNOWN
 Keywords: tala tdm ddd ddds dialogue conversation AI
 Platform: UNKNOWN
@@ -14,15 +14,14 @@
 Requires-Dist: Jinja2 (~=2.10)
 Requires-Dist: pathlib (==1.0.1)
 Requires-Dist: lxml (==4.2.5)
 Requires-Dist: iso8601 (==0.1.12)
 Requires-Dist: python-magic (==0.4.15)
 Requires-Dist: prompt-toolkit (==2.0.8)
 Requires-Dist: requests (==2.21.0)
-Requires-Dist: typing (==3.7.4.1)
 Requires-Dist: structlog (==18.2.0)
 
 This is a command line SDK for managing TDM-based dialogue domain descriptions (DDDs). For further information, see [talkamatic.se](http://talkamatic.se).
 
 # Install dependencies
 Ubuntu LTS 16.04 is supported. Install non-python dependencies with `apt-get`:
 ```bash
```

## Comparing `tala-8.0.0.dist-info/RECORD` & `tala-9.0.0.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 bin/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 integration_tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-integration_tests/test_console_scripts.py,sha256=1WUp8xQ7XBXOs_0UeCvCOl3dcUnEv2G2AHaZf1TOHvI,31685
+integration_tests/console_script_mixin.py,sha256=9fFKhgkCEeB9X3SLrzvooiToGbqAeNy47WlxCkSdKfk,5995
+integration_tests/expected_generate_rasa_output.py,sha256=JsdP-_cbBe3daQZA7V5Xw8HuaGXBWTHojEqVGQpopPc,9007
+integration_tests/test_create_configs.py,sha256=wTI3-SU_7J3T0f-T4eJ3pEhT5ddDfy-k9DNRcw7krCE,4937
+integration_tests/test_create_ddd.py,sha256=1J0sne0FtmKrXi_slwxLYpIiScz0tOQuSZ7107Lzsxg,983
 integration_tests/test_ddd_py_to_xml.py,sha256=2iO8LH5yzUDEXUCVN-aogV5wpnItu-7Fqzt7w5fWT00,7668
 integration_tests/test_ddds.py,sha256=a2d6qGQJ00UuAEzyl3hSBYlOwrj1RU5nCCFVlmlSx80,1241
+integration_tests/test_generate_alexa.py,sha256=T0aBJCIEFm5sHoWm0SEnkHQIu4UrwCHQYNugcfcgi_A,8571
+integration_tests/test_generate_rasa.py,sha256=kHVyjqz61nJ_NU5BmXC7h_FcWDrfTWf8mX6mPK_H0JU,6969
+integration_tests/test_interact.py,sha256=EsEtdOHhkijSNCFqqqidPXQ0jG9BFSwUYC6KahpiIPo,555
+integration_tests/test_verify.py,sha256=V-IAiaFlvA9lUMXSBMSaCBpPs9OPSbvNSqX_wmXuKWg,4296
+integration_tests/test_version.py,sha256=kRMXX0L9J4U5iyVYMH709_9_uqM_kNX-gAcqSWqFyJ8,1053
 tala/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tala/config.py,sha256=Q2djGQMNdBKUdcXe5G36q_CqOqi_zPvfhTxTSFZ8Av4,11134
-tala/installed_version.py,sha256=NPFvBkS-6IHCuPrpM-DmUyHFvgS86-SHOj4xiyRtbdo,116
+tala/installed_version.py,sha256=aj7r_JdEANWcPFXhmQjP55ZgOZLvozNt4vDrfQLUdIY,116
 tala/backend/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tala/backend/dependencies/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tala/backend/dependencies/abstract_backend_dependencies.py,sha256=BT1MsxT4T4dD7ZSogHAL9YbQ6oLUYV8KOrGQwnNy8KY,3048
 tala/backend/dependencies/for_generating.py,sha256=QhmpZIiu8nIc_pJhhG8bm6Y6e_QbU38c-ViIPYPCZ2Y,1605
 tala/cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tala/cli/argument_parser.py,sha256=cN31Cy_CtogXBsQ1U90NhzzjgqTA-_9x51kwgLSXmQc,877
 tala/cli/console_formatting.py,sha256=CPJPuAexX1XsOjg2uWmHMkKFFSe9BI5tq0mpHPWQnwA,629
-tala/cli/console_script.py,sha256=SU-fwiJIDMRXimA59Ga6tENbG_PaJCm_covuSVEcgDs,14828
+tala/cli/console_script.py,sha256=22RcesPWvZ77PqXSoKHJEuIBNJmwWgml9LO0Wm9vy90,15691
 tala/cli/tdm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tala/cli/tdm/passivity_timer.py,sha256=GexICzPNbux5KsMPKcsLnnNk7CqoW-X7Pl7yLb1p8as,459
 tala/cli/tdm/tdm_cli.py,sha256=hFQtWNc70aXnHIlbSCFUi2fxGPZU15UO5VRWJy2mYgI,2800
 tala/ddd/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tala/ddd/ddd_py_compiler.py,sha256=nI9eigcVOp98is33wj339JeJqN0uJnPGKD0O8IDBNIk,20856
-tala/ddd/ddd_xml_compiler.py,sha256=2c_9h_1ewAqTLCULazXs0nVunhLKYiNj94wsAm6531w,51241
-tala/ddd/parser.py,sha256=be868vQ2xoM9GNmrpyFWkor0wLpwh7Hdt_VJ1Qg48dU,46160
+tala/ddd/ddd_xml_compiler.py,sha256=vmFwlPwfabxr_mCb1Uj_EIiftvmKA5v6OS50aReSSpk,51080
+tala/ddd/parser.py,sha256=qwTf9hQk4plrBt2GBpgYzw3rNqReGgilkH68Hokwdj0,46752
 tala/ddd/utils.py,sha256=pdelLTmbPVoV_uo6QCn96bwg8byNRwUOEhwMyukP9Vc,1428
 tala/ddd/building/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tala/ddd/building/ddd_builder_for_generating.py,sha256=eSMPcQq1-bn2tWtgw5Fv0m82i2XAtQFUw6kE2DeT2Gg,2713
 tala/ddd/building/supported_asrs.py,sha256=R__tH1WRkIb4mR0AM2ohxVeiovmE51aAlFjg0OuJrtw,94
 tala/ddd/building/steps/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tala/ddd/building/steps/abstract_build_step.py,sha256=ST3FquNfNEyPRt2K2AprgVsUgnjgupkDryUTOsNpUkU,522
 tala/ddd/building/steps/clean.py,sha256=l7m-Zs7MsEaaVTNiAAuyPUM_OyaYL4tTcocf1a0cwJ4,1497
@@ -45,15 +53,15 @@
 tala/ddd/maker/templates/domain_template.xml,sha256=BAgbTz67Wfg3ImsGk_CSWyj-xOo2dbkvqjrPtJDmn8w,221
 tala/ddd/maker/templates/grammar_eng_template.xml,sha256=9y3vgE9Fxp9QeP5GWpc207YdvhONvrQkd1aFJkgFBrs,60
 tala/ddd/maker/templates/interaction_tests_eng_template.txt,sha256=earZrXBX2arbU7bKtXkSxUYspjiZ7Fl1YVdwjbcFwX8,44
 tala/ddd/maker/templates/ontology_template.xml,sha256=OnPzV1fssl4yw7gX5QTCUTpqNva_FEZ1QZfmP4Mpj34,85
 tala/ddd/maker/templates/service_interface_template.xml,sha256=0OVDsmsfiyfKwPxTyqTYyowIUNwxDmg-FPHbYY_wwKA,80
 tala/ddd/maker/templates/word_list_template.txt,sha256=L6zUk3sUVhq6KjWjl8e5JfadLOLMxIBk_1a0ySWZb6c,191
 tala/ddd/schemas/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tala/ddd/schemas/domain.xsd,sha256=2b36yJJoXMqkeeQmeaZucsjEvQfukZM4zyUo4UXT9cI,14080
+tala/ddd/schemas/domain.xsd,sha256=rjZHPwafnDt9LaaLlgnSZt01zFMt6awK7CCUN-yrOF8,14130
 tala/ddd/schemas/grammar.xsd,sha256=No6ZT7VBhRZesHvGje54sDaDwisxgi9kGtNE42fBnOg,11072
 tala/ddd/schemas/grammar_rgl.xsd,sha256=6daZ58zxNxQc6UxeahSGn7saC6qXJmoML0vk5BFfdxY,6444
 tala/ddd/schemas/ontology.xsd,sha256=lQiLu7xUiyRSfE0dxIdKUqiAi3KZkDmElFoNL9oDDEc,1801
 tala/ddd/schemas/service_interface.xsd,sha256=GTcRe754UTAxpBHoCr7iC1FPUVV0iPd3tTEIND09AVo,7890
 tala/ddd/services/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tala/ddd/services/constants.py,sha256=n12YduZx-p4byhMkOqxHlHxofXySUoyMkcDV4HINxmQ,55
 tala/ddd/services/service_interface.py,sha256=gDr-DpkWpwCmIsEaRM2Couf6g0Jw4pZDmWdBG320jIs,13020
@@ -125,18 +133,21 @@
 tala/ddds/small_grammar/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tala/ddds/small_grammar/service.py,sha256=nVXlcX9L0oK2KHxeIzz6n8f4VmzC-jlNsDVf8MBTzfY,273
 tala/ddds/small_grammar/grammar/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tala/ddds/tidePooler/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tala/ddds/tidePooler/device.py,sha256=b-MnlSQORB7ALNit2IvWkXjcka7YDv2Y2vXS3zYF-cM,2811
 tala/ddds/tidePooler/grammar/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tala/log/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tala/log/extractor.py,sha256=2KiG5aqng65HGYZFn1exqZu-Rgi8O24MYE_Tx_MzdLs,2866
+tala/log/interaction_test_extractor.py,sha256=AW0ZGVWd1afNs1G60zXDJvW3uqQ1Owb2kSHQ_uFF1II,9492
 tala/log/logger.py,sha256=LMdCAlL0pGcouXzjQvLtTnVilbFUquBTzx8yHmNt9zM,1557
+tala/log/serialization.py,sha256=dyO3M1tOWo46SpIs2QDahA0zAck-MurUzQEOzJcPZmA,168
 tala/model/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tala/model/action.py,sha256=YPCTsrpXVyVwhxa-AwVncYy_rI0Eta3vq5VdGzidic4,1320
-tala/model/action_status.py,sha256=gchHZ-5egQOtfWt62ne4BYSUhbB1B6UMShnAK435hiY,259
+tala/model/action_status.py,sha256=a4wfX0aGlbKGHco1WMR1Ypwsatsm-sH5rdOnmeogtv4,370
 tala/model/ask_feature.py,sha256=h_unc5qtvpQb_otDLnDNRTcNGHIYNqrauIjaOsj8QrU,215
 tala/model/audio_directive.py,sha256=bvHYFUHD6DLzWIgaoixc98xaIlkFTtcz6hk7u1V5dGs,910
 tala/model/common.py,sha256=x5pNqxjVD_qCLBrJbG37MN2b2TQRBBoWIMZGX0HISQg,287
 tala/model/condition.py,sha256=bcXDEPbZvm0wQn7rL1ijB6_mBcoKYAzZyb_QQuMzfPc,1793
 tala/model/database.py,sha256=tBnvubkDmyxsd0_u0StzHX4LaaRo2TMgXNk_HR6Xh_E,506
 tala/model/date_time.py,sha256=1roHwiRGJvgq6ttNhpdiSYYv4oSRmRkn5srp-RKGJ7U,1395
 tala/model/ddd.py,sha256=leTfKpy8Hnm-QTjvM6jcJYf7VINtFP_WmX4QGIfINZg,1755
@@ -144,26 +155,26 @@
 tala/model/domain.py,sha256=MsrC4asmrxg72vx4FYtpCpXdt8BMGTWZmCfC_pfrtAM,14070
 tala/model/entity.py,sha256=THSGsWUgj3eLps7MfVrW4LHGKc7e9zCvyyf8J-O2hIE,952
 tala/model/error.py,sha256=OCRWb9qfXUAzk3eTpw2dyJK5Vg1wdLNZGjec04Q5PUM,82
 tala/model/event_notification.py,sha256=-NsOU5Qks5MTDts32fzSKOLTTTBCpXkLsnJS5nWjM3g,1069
 tala/model/goal.py,sha256=UHDL3DJm1ACuWFz1T6rlmCXeP0fzbElmtjNym2tlL-k,5324
 tala/model/image.py,sha256=n3ovOWWXSyCnh92RHUUei2vzGesLSHifjnfXzGZHN3Y,549
 tala/model/individual.py,sha256=0RuOwFHWPPBjUgA2QRYfQAzwh0LCQkomx94We2nB9bY,3566
-tala/model/input_hypothesis.py,sha256=6gtHztg-nJlLAWdP0CMb6AjSvrFjxOLUYzTWm03OWHo,766
-tala/model/interpretation.py,sha256=SKD-DToAsDu53wQLFKVGJIhi5uhTgMOubd-_361fsXA,2281
+tala/model/input_hypothesis.py,sha256=JMoiSzxwn0innSWxXEbPfpVZ83eTAYcAIc2J7T-Jy94,950
+tala/model/interpretation.py,sha256=2kYZcDmzJUbna_iC6rO36uYat8YSaV4t2PE9cZ5bGQE,2551
 tala/model/lambda_abstraction.py,sha256=Bld-ChQsUGZtrs8JT3eENm3l1qwthXjcq4giGQuKQ14,2643
-tala/model/move.py,sha256=2pbwKta0FuMllJIZGKoabT68XjctFdNdo_8G2SAs4YI,20382
+tala/model/move.py,sha256=4wvtMbl_VyOfC3IVNpd0mNQlfSejDCRWZcVW7j2IlLs,20373
 tala/model/ontology.py,sha256=478A8gRp0ma-Mnqgnmz7gF-SKJ1WRLrmGZr75JhCBNs,10528
-tala/model/openqueue.py,sha256=HbcliyTE4M6AQSJZ4gWVBgr3yspkHZSw1iA30-d7uCQ,4461
+tala/model/openqueue.py,sha256=tj5zggq1i99gw-wVUu6Jisjpcl73CcVjQTLZ1URyGV4,6821
 tala/model/person_name.py,sha256=MieRb4VXcy-1Wx62i2WHAiYRNern1IRHpRKBaZd29Qw,352
-tala/model/plan.py,sha256=bU64tH0vGt01NmZS-F4jrRTgKv8KZ-t3c2p2WuZ_aXc,2987
-tala/model/plan_item.py,sha256=p03j5MxIFb2F_FRYOT7pBh97AbPf85DSCeF0Rnx6e3s,15493
+tala/model/plan.py,sha256=XesHl4oJnkpITB9HI6lu0arYHYF7IsIGX7hE65geFHA,3411
+tala/model/plan_item.py,sha256=VVHyuG4LzHCvm696CJKCWg820sfOyKpB6kQV59d41Nc,16223
 tala/model/polarity.py,sha256=CZHmfMUvH7lZJbuOX1reFBLhsToO3rJELwvqPyAv3RE,48
 tala/model/predicate.py,sha256=re5wPTzkO7KD6SFxelQucuJ57rZYIAK0E1IQTlX8txA,1795
-tala/model/proposition.py,sha256=aeNGQo5B_vGu2_OSm1wgY6OlSqW0-N8N79MkuJ-5HTk,26904
+tala/model/proposition.py,sha256=6D6nSVx5sCbO3oDC9Kf2DMEp8O_swgn_RyryXUNHLjo,27132
 tala/model/question.py,sha256=_wnKxlIoazv8dXgsU3EKTpsdrhMXTKyDjlKLua81OkI,3795
 tala/model/question_raising_plan_item.py,sha256=vqPcCckjYSF2URNAi-UYOVwO2AUNERyyTmzHbE7Yo60,3390
 tala/model/semantic_object.py,sha256=YPMOwfFl6jnoq5-WTl7yf58BCLvmcJDll9yj4fVt7NY,1980
 tala/model/service_action_outcome.py,sha256=QTPhmUmj0WCtjAU8YubsFhhXvDVS67gpO5FrSRdxgAE,1254
 tala/model/service_invocation.py,sha256=GFno71BhEw2F8oNhxRa5qnFvP3xdlo_k50J2jEMHO1A,229
 tala/model/service_query_result.py,sha256=hZ-gMkHcS-0jh7iy7TTWrlROJ01X9P8d_qKhgcDvsMI,485
 tala/model/set.py,sha256=GVrja0AVXAiQ2YOUXZg9ookNt25R5u_JktCzSn80wkk,2865
@@ -176,18 +187,18 @@
 tala/model/validation_result.py,sha256=xRYQdUhT9tus-mHnsJTtouZKib3hyomOhcEttb1YL3c,1318
 tala/model/webview.py,sha256=DFymK6HVsxq8O2yHY5wf6WpiM7Yx2G0cSbNN5vJykjw,553
 tala/model/grammar/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tala/model/grammar/grammar.py,sha256=ptg5qP-6DEy31TRB-8osXTENyF80WGBmMSe-kh-ZLsU,12825
 tala/model/grammar/intent.py,sha256=tujEqThFVY85dcJ8Bt5klH306pMBmOBI_QTi-RMJoo8,2329
 tala/model/grammar/required_entity.py,sha256=R8Prg91CgM1bVO7zQxuA0i8zGulhNNl1JOwBJ5DhxZg,788
 tala/nl/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tala/nl/abstract_generator.py,sha256=s9cEZUq8Q9IXahYap1urRNzYXVaZcTgg1DtYM6Zuo20,5802
+tala/nl/abstract_generator.py,sha256=nmLGZCJxiS5VAcXPnfRVmBiB-9KxhoTwsTMsf-4hSDI,5832
 tala/nl/constants.py,sha256=laErVW-JNbiT428psLmABEjcT5fqYYkN1XgxXuL7mic,409
-tala/nl/examples.py,sha256=TdpXCY2zqstpNVEJqxASehFLv9hmDQZSCPUiJSySXeA,19298
-tala/nl/generated_intent.py,sha256=oipmyKDdpQ1nraNO-P_pFquLM7wkbBUsvRWrp89rfoE,516
+tala/nl/examples.py,sha256=NuqQ-AW-GQqLD3G-AsGuGmF2oLAhQmlCMr40UBPO3Tg,21934
+tala/nl/generated_intent.py,sha256=MWLSJUvKZDwehN_gwcrCpg-E7hn1McVP7mut3vpHTS8,1181
 tala/nl/languages.py,sha256=Wlrg98IxJTKkrEm9tJL7y0s2SX6UdZyEMMzWmHTzF4U,531
 tala/nl/selection_policy_names.py,sha256=NKruB6xPuJDQIIpIN3C0vkvhQXL3Vr9YMAUGgGwThW8,40
 tala/nl/alexa/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tala/nl/alexa/generator.py,sha256=zYopBhREVzVwpDRGAcDcV90X_lM75oqrDkMq68kxmHU,7919
 tala/nl/gf/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tala/nl/gf/auto_generator.py,sha256=BOP3cUM61Ko-rUeJAnefvwhyd2TsIiW0ICMFu20iNWY,76716
 tala/nl/gf/grammar_entry_types.py,sha256=yHYPgk3ltcqkMZPwtJLZfPH5w16MhYB3eOyBCO6N0iA,2742
@@ -196,43 +207,43 @@
 tala/nl/gf/resource_eng.py,sha256=1IWeMAiF7mNywtjHvyBFrSfwkVGFmAXqeMPmVf5DyIU,164
 tala/nl/gf/resource_it.py,sha256=rp_wW2gHOkLAaLiC8x8BJp-0lp_rvSJ6KTF9OgXKHBU,460
 tala/nl/gf/resource_sv.py,sha256=zK4coAb4wm7gFjSFTWYHU7VvT0NGNrplTJwZvMwKjQ4,98
 tala/nl/gf/rgl_gf_generator.py,sha256=Vht3IxOYjBPV0KGkxR5JKdgBT7EA4ogDKB4jLHy40nw,51072
 tala/nl/gf/rgl_grammar_entry_types.py,sha256=JyQdxcweILJylOAFB-O4Jdykk0qAZISDf0T7rC4E5og,222
 tala/nl/gf/utils.py,sha256=AxgN0pEIy6ijzVUQitnF5152Z7tTlslOWiCKbFMEY8s,5162
 tala/nl/rasa/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tala/nl/rasa/generator.py,sha256=elLt1vsJRjlE4zOVPDxMTKDE2IIsNezC85kLDn695mw,10474
+tala/nl/rasa/generator.py,sha256=k9jwRqOlVOm0wd_VKx5oOJGRoQa-WGWOtU2HOFnsKlU,10957
 tala/testing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tala/testing/backend_dependencies_test_base.py,sha256=pc85RoFuuNq_qxXptIyiAKm-9PlWI_cSkTuxnIeYqkU,2168
 tala/testing/ddd_mocker.py,sha256=fOq5pCQiXksfC5sHRRiFqpwhbZk8GO_6EdAa6QdYujU,3698
 tala/testing/lib_test_case.py,sha256=4HakpxJLCY2nPc_9Ikh4iQDQfAOMmZlYQFGwEsRB-5o,6991
 tala/testing/move_factory.py,sha256=cS6u5vUhD8RXYrZFHHVDTocbFtZ2bbYTML13GaezPKI,4750
 tala/testing/utils.py,sha256=sNXmtrhm0_V8nUi_8rU1CzqrfAzaI_Ze-Bdb2Oi1dAg,517
 tala/testing/endurance/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tala/testing/endurance/named_test.py,sha256=wo9hq_cVtsHSwbfg_rwWD5ftgm0o6SpkCn1_AWSp9_Q,1958
 tala/testing/endurance/runner.py,sha256=nUOf4WFX0sLLv-HiYFSStlbo7s5bci8MVZhjdkcJROM,1488
 tala/testing/interactions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tala/testing/interactions/base_test.py,sha256=1cvo6nIQ88EvJwKTuTDpR1sWbsz6MYaTYVBnfYJfIXc,411
-tala/testing/interactions/compiler.py,sha256=0zARfDwjT4bcSnVNKkoLxAkXjTSorrHlpHIf9hnTJDQ,8400
+tala/testing/interactions/compiler.py,sha256=d4z16HkAaPo1rlmS2shw4upHXASynfm7mha9FynKRWY,10007
 tala/testing/interactions/file.py,sha256=TbhoNXOwK80eBy2PZx3Q-hXM1lDnUedt3DVX8TRkioQ,1840
 tala/testing/interactions/named_test.py,sha256=on36Q5NRRDb9Ytvl92lPyvo4_rHqqkUGxdRNmZzvH68,466
 tala/testing/interactions/result.py,sha256=nQbQDNcvTX5x5kgJ6gsNIIFEXhyVaxzL-B062zjfjdU,946
 tala/testing/interactions/suite.py,sha256=w7dMrjHpYblpKhH0Qzl8iFZDOq5HEF5wcOkWJUM8fxk,219
-tala/testing/interactions/testcase.py,sha256=Zp7J93O7I00P-wXTHePsoSoe6th8qv4rx9T9ablNL3Y,12028
+tala/testing/interactions/testcase.py,sha256=GtZs4i_pL6TXJ3dd4ojhFbzM9nAfoPU_-kRJbAQ3prM,12957
 tala/testing/interactions/testloader.py,sha256=p7v-eCO0MAYAnDEe5_3wiIKNFR8jv859i6XNRzBFg2A,679
-tala/testing/interactions/turn.py,sha256=RvNvvVbGl7IxIngQZ1MjRf_FTTvHPKhti0Z84_IEzHk,3654
+tala/testing/interactions/turn.py,sha256=gUCmt1FUysZAzxUScsg1nAlDAtovknpCp4k_seofBdI,4075
 tala/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tala/utils/as_json.py,sha256=Z67HPZ3pluqAv3E_L37wYIb1AhYST7WJvZ9106jj8Ro,1448
 tala/utils/as_semantic_expression.py,sha256=n5xO-r8jzyq04DfK8GGrcAN78dwBPrF1sA3v5e5M38s,104
 tala/utils/await_endpoint.py,sha256=xR-4Q2gwe0ZFwjwVLDg-Y0CmDmN7Fo21uij0ldQ35NE,676
 tala/utils/chdir.py,sha256=zv87kyf41qDkfZtLBWC50Q49c0LPYfdHJtyyAJK3RU0,383
 tala/utils/equality.py,sha256=YhsgXA3pQCcpz08gFwLnK_4kufQGMYwWbtJuSmbF4Vo,917
 tala/utils/float_comparison.py,sha256=m01aCDql4YH9hk784PC53UXoJuYAwIcJXbV6otsHYxA,612
 tala/utils/observable.py,sha256=r1CsAaajHt3JXiP9Xqy_aGrHXojlTRZfdwIz4Pt5gKM,466
-tala/utils/tdm_client.py,sha256=yLDIhAaEW4JoTT7vDH1m__ELpPZVNMclZ0KBOb2bxe8,5625
+tala/utils/tdm_client.py,sha256=EcPEm40Wlcwkx4D3cNQ4vtGecu-it82UBAep3mvQVF8,5722
 tala/utils/unicodify.py,sha256=Q-JGJ0m-mlA2WfWkwQn_wG9J_9AleH6j7wKXak8sOLA,1034
 tala/utils/unique.py,sha256=V9aQL-crvQWuSkoJD3diwK6L0b_RwEOMe90reC8MV_g,108
-tala-8.0.0.dist-info/METADATA,sha256=IkiSdMcnpP_bhZHDH47r5dtH_yDg0rCpTqDgPYzO3mE,1301
-tala-8.0.0.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
-tala-8.0.0.dist-info/entry_points.txt,sha256=-QNxI3q_TTeafmydwBpqMIGuYpt2YVZNDOoQMDhK2dg,55
-tala-8.0.0.dist-info/top_level.txt,sha256=ZN3QCyEASrHwtSaq3G8qsR1pNVwFzi9F8uffLEa3WnM,27
-tala-8.0.0.dist-info/RECORD,,
+tala-9.0.0.dist-info/METADATA,sha256=sCgRZEMLinia-kzXpMraj7LdblYddIWDdE4O8-4ki2E,1267
+tala-9.0.0.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
+tala-9.0.0.dist-info/entry_points.txt,sha256=-QNxI3q_TTeafmydwBpqMIGuYpt2YVZNDOoQMDhK2dg,55
+tala-9.0.0.dist-info/top_level.txt,sha256=ZN3QCyEASrHwtSaq3G8qsR1pNVwFzi9F8uffLEa3WnM,27
+tala-9.0.0.dist-info/RECORD,,
```

