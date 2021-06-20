# MicrosoftDesafiosIA
Desafios do Curso de Inteligência Artificial da Microsoft

*Para saber sobre os passos realizado em cada desafio acesse:* </br>
*[Desafio 1](https://github.com/DiegoRib/MicrosoftDesafiosIA/blob/main/Desafio1.md)*</br>
*[Desafio 2](https://github.com/DiegoRib/MicrosoftDesafiosIA/blob/main/Desafio2.md)*</br>
*[Desafio 3]()*</br>
*[Desafio 4]()*</br>

### Desafio 1 - Existe alguma correlação entre as notas das provas objetivas? Comente.

Input: 

    NU_NOTA_CH = 0
    NU_NOTA_LC = 0
    NU_NOTA_MT = 785
       
Output:

    Predicted Nota: 254.40

***Obs: para a IA retornar alguma previsão é necessario enviar a nota das 3 competências, caso uma das notas fique como null é exibido a seguinte mensagem de erro.***

    The request failed with status code: 400
    Access-Control-Allow-Origin: *
    Content-Length: 2282
    Content-Type: application/json
    Date: Sun, 20 Jun 2021 02:18:46 GMT
    Server: nginx/1.14.0 (Ubuntu)
    X-Ms-Request-Id: d049f046-2af9-4564-a4ad-26125f1753eb
    X-Ms-Run-Function-Failed: False
    Connection: close

    {'error': {'code': 400, 'message': 'Input Data Error. Input data are inconsistent with schema.\nSchema: {\'columnAttributes\': [{\'name\': \'NU_NOTA_CH\', \'type\':
    \'Numeric\', \'isFeature\': True, \'elementType\': {\'typeName\': \'int64\', \'isNullable\': False}}, {\'name\': \'NU_NOTA_LC\', \'type\': \'Numeric\', \'isFeature\': True, 
    \'elementType\': {\'typeName\': \'int64\', \'isNullable\': F\nData: defaultdict(<class \'list\'>, {\'NU_NOTA_CH\': [None], \'NU_NOTA_LC\': [None], \'NU_NOTA_MT\': 
    [785]})\nTraceback (most recent call last):\n  File "/azureml-envs/azureml_2439cbd4ba441d4c922a33cfeff2215c/lib/python3.6/site-
    packages/azureml/studio/common/datatable/data_type_conversion.py", line 61, in convert_column_by_element_type\n    return _convert_column_of_all_missing_values(column, 
    new_type)\n  File "/azureml-envs/azureml_2439cbd4ba441d4c922a33cfeff2215c/lib/python3.6/site-packages/azureml/studio/common/datatable/data_type_conversion.py", line 337, in 
    _convert_column_of_all_missing_values\n    raise ValueError(f\'Cannot convert column of all missing values to {new_type} type.\')\nValueError: Cannot convert column of all 
    missing values to int64 type.\n\nThe above exception was the direct cause of the following exception:\n\nTraceback (most recent call last):\n  File "/azureml-
    envs/azureml_2439cbd4ba441d4c922a33cfeff2215c/lib/python3.6/site-packages/azureml/designer/serving/dagengine/dag.py", line 167, in execute\n    input_data = 
    create_dfd_from_dict(raw_input, schema)\n  File "/azureml-envs/azureml_2439cbd4ba441d4c922a33cfeff2215c/lib/python3.6/site-
    packages/azureml/designer/serving/dagengine/converter.py", line 28, in create_dfd_from_dict\n    converted_column = convert_column_by_element_type(column, target_type)\n 
    File "/azureml-envs/azureml_2439cbd4ba441d4c922a33cfeff2215c/lib/python3.6/site-packages/azureml/studio/common/datatable/data_type_conversion.py", line 98, in 
    convert_column_by_element_type\n    base_error=e)\n  File "/azureml-envs/azureml_2439cbd4ba441d4c922a33cfeff2215c/lib/python3.6/site-
    packages/azureml/studio/common/datatable/data_type_conversion.py", line 320, in _raise_convert_type_error\n    raise convert_type_error from base_error\nTypeError: Cannot 
    convert to type "int64": Cannot convert column of all missing values to int64 type.\n', 'details': ''}}
