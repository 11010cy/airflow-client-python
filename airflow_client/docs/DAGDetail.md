<!--
 Licensed to the Apache Software Foundation (ASF) under one
 or more contributor license agreements.  See the NOTICE file
 distributed with this work for additional information
 regarding copyright ownership.  The ASF licenses this file
 to you under the Apache License, Version 2.0 (the
 "License"); you may not use this file except in compliance
 with the License.  You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

 Unless required by applicable law or agreed to in writing,
 software distributed under the License is distributed on an
 "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 KIND, either express or implied.  See the License for the
 specific language governing permissions and limitations
 under the License.
 -->

# DAGDetail

DAG details.  For details see: [airflow.models.DAG](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/models/index.html#airflow.models.DAG) 

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dag_id** | **str** | The ID of the DAG. | [optional] [readonly] 
**root_dag_id** | **str, none_type** | If the DAG is SubDAG then it is the top level DAG identifier. Otherwise, null. | [optional] [readonly] 
**is_paused** | **bool, none_type** | Whether the DAG is paused. | [optional] 
**is_active** | **bool, none_type** | Whether the DAG is currently seen by the scheduler(s).  *New in version 2.1.1*  *Changed in version 2.2.0*&amp;#58; Field is read-only.  | [optional] [readonly] 
**is_subdag** | **bool** | Whether the DAG is SubDAG. | [optional] [readonly] 
**fileloc** | **str** | The absolute path to the file. | [optional] [readonly] 
**file_token** | **str** | The key containing the encrypted path to the file. Encryption and decryption take place only on the server. This prevents the client from reading an non-DAG file. This also ensures API extensibility, because the format of encrypted data may change.  | [optional] [readonly] 
**owners** | **[str]** |  | [optional] [readonly] 
**description** | **str, none_type** | User-provided DAG description, which can consist of several sentences or paragraphs that describe DAG contents.  | [optional] [readonly] 
**schedule_interval** | [**ScheduleInterval**](ScheduleInterval.md) |  | [optional] 
**tags** | [**[Tag], none_type**](Tag.md) | List of tags. | [optional] [readonly] 
**timezone** | **str** |  | [optional] 
**catchup** | **bool** |  | [optional] [readonly] 
**orientation** | **str** |  | [optional] [readonly] 
**concurrency** | **float** |  | [optional] [readonly] 
**start_date** | **datetime, none_type** | The DAG&#39;s start date.  *Changed in version 2.0.1*&amp;#58; Field becomes nullable.  | [optional] [readonly] 
**dag_run_timeout** | [**NullableTimeDelta**](NullableTimeDelta.md) |  | [optional] 
**doc_md** | **str, none_type** |  | [optional] [readonly] 
**default_view** | **str** |  | [optional] [readonly] 
**params** | **{str: (bool, date, datetime, dict, float, int, list, str, none_type)}** | User-specified DAG params.  *New in version 2.0.1*  | [optional] [readonly] 
**any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


