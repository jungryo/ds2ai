

The official [DS2.ai](http://ds2.ai/) SDK for Python.  
Documentation can be found on [SDK guide](https://docs.ds2.ai/sdk_00_readme.md)

# MLOps with DS2.ai

[DS2.ai](http://ds2.ai/) is an integrated AI operation solution that supports all stages from custom AI development to deployment. It is an AI-specialized platform service that collects data, builds a training dataset through data labeling, and enables automatic development of artificial intelligence and easy deployment and operation.

The Software Development Kit (SDK) consists of python functions that allow you to write your own scripts by accessing DS2.ai's features.

![Screen_Shot_2021-07-01_at_3 37 53_PM](https://user-images.githubusercontent.com/72846894/124224623-fcc39c80-db40-11eb-9737-2e384d88c300.png)

## Installation

---

Install via pip:

```
$pip install -i https://test.pypi.org/simple/ ds2ai==0.20
```


## Getting started

---

### 1. Getting your own token

To use the SDK, you need to get a token, and you can check the token by registering as a member of [console.ds2.ai](http://console.ds2.ai/). After registering the card on the site, you can use the token.  

<center>
<img width="2000" src="https://user-images.githubusercontent.com/72846894/124224654-0b11b880-db41-11eb-8764-90dc1d2cf469.gif"/>
</center>

### 2. Activate

To use SDK function code, you have to activate your code, first.

Run the below code with your own app token. 

```python
import ds2ai

ds2 = ds2ai.DS2(token)
```

Then you can use all functions in [DS2.](http://ds2.Au)ai SDK.

## Top 5 Features of [DS2.ai](http://ds2.ai/) SDK 

---

The SDK is composed of 16 classes. Class DS2 provides python functions that are more generally used for AI development, whereas the others provide specific functions for each detailed steps in AI development.

Here, we want to explain to you examples of using **Top5 function codes that are usable and easy to use.** 

### 1. Auto Labeling

Executes auto-labeling immediately from loading data file without using dataconnector.

```python
ds2.start_auto_labeling(data_file, amount, has_label_data=False, predict_column_name=None,
            frame_value=60, ai_type="general", autolabeling_type="box",
            general_ai_type="person", model_id=None, custom_ai_stage=0, 
            preprocessing_ai_type={}, labeling_class=None, workapp="object_detection")
                          
```
<img width="2800" src="https://user-images.githubusercontent.com/72846894/125379543-a883ac80-e3cb-11eb-8db3-19dbc2c1b859.gif"/>


### 2. AI Training

Executes development of Click AI immediately from loading data file without using dataconnector.

```python
ds2.train(data_file, has_label_data=False, frame_value=60, training_method=None, 
    value_for_predict=None, option="accuracy"))
```
<img width="2800" src="https://user-images.githubusercontent.com/72846894/125380537-4c218c80-e3cd-11eb-85e7-cb8686f2cf7b.gif"/>

### 3. Deploy your AI model

Deploys AI models to cloud servers with specifications under the desired hosting region.

```python
ds2.deploy(model_file, name=None, cloud_type="AWS", region="us-west-1", 
    server_type="g4dn.xlarge")
```
<img width="2800" src="https://user-images.githubusercontent.com/72846894/125379607-c7823e80-e3cb-11eb-85ce-c0cd35cfa588.gif"/>   


### 4. Getting magic code

Returns a the magic code for setting variable values ​​with optimal combinations for AI training.

```python
ds2.get_magic_code(data_file, has_label_data=False, 
            frame_value=60,training_method=None, value_for_predict=None)
```
<img width="2800" src="https://user-images.githubusercontent.com/72846894/125379392-68242e80-e3cb-11eb-858b-bd005085a501.gif"/>   


### 5. Rent AI training server

Rents an inference training server in prefered cloud environment for Custom training of Click AI

```python
ds2.rent_custom_training_server(cloud_type="AWS", region="us-west-1", 
                        server_type="g4dn.xlarge", name=None)
```
<img width="2800" src="https://user-images.githubusercontent.com/72846894/125380727-9efb4400-e3cd-11eb-824b-676d670941b5.gif"/>   


## **Getting Help**

You can interact with the ds2ai code or software by asking a question or referencing the guide from the underlying open resources.

- GitHub
    - [https://github.com/DS2BRAIN/ds2ai](https://github.com/DS2BRAIN/ds2ai)
- stackoverflow - Ask all code and software related questions here.
    - [https://stackoverflow.com/questions/tagged/ds2ai](https://stackoverflow.com/questions/tagged/ds2ai)
- CrossValidated - Ask questions about artificial intelligence algorithms and theories here.
    - [https://stats.stackexchange.com/questions/tagged/ds2ai](https://stats.stackexchange.com/questions/tagged/ds2ai)
- Documentation
    - ds2ai user guide : [https://docs.ds2.ai/](https://docs.ds2.ai/)
    - ds2ai blog : [https://blog.ds2.ai/](https://blog.ds2.ai/)
- Website
    - [https://ds2.ai/](https://ds2.ai/)

If you need help that is not specific to this SDK, please reach out to the chat "Ask us in [console.ds2.ai](http://console.ds2.ai).

## **License**

This SDK is distributed under the Apache-2.0 License, please see [LICENSE](https://github.com/DS2BRAIN/ds2ai/blob/main/LICENSE) for more information.

<br>
<br>
<br>
