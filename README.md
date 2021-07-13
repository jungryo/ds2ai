![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FDS2BRAIN%2Fds2aihit-counter&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)

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

![get_token (1)](https://user-images.githubusercontent.com/72846894/124224654-0b11b880-db41-11eb-8764-90dc1d2cf469.gif)


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

가이드 링크

With just a single function code execution, you can get the data loading, project creation, and results of auto labeling.

```python
ds2.start_auto_labeling(data_file, amount, has_label_data=False, predict_column_name=None,
            frame_value=60, ai_type="general", autolabeling_type="box",
            general_ai_type="person", model_id=None, custom_ai_stage=0, 
            preprocessing_ai_type={}, labeling_class=None, workapp="object_detection")
                          
```

### 2. AI Training

```python
ds2.train(data_file, has_label_data=False, frame_value=60, training_method=None, 
    value_for_predict=None, option="accuracy"))
```

### 3. Deploy your AI model

```python
ds2.deploy(model_file, name=None, cloud_type="AWS", region="us-west-1", 
    server_type="g4dn.xlarge")
```

### 4. Getting magic code

```python
ds2.get_magic_code(data_file, has_label_data=False, 
            frame_value=60,training_method=None, value_for_predict=None)
```

### 5. Rent AI training server

```python
ds2.rent_custom_training_server(cloud_type="AWS", region="us-west-1", 
                        server_type="g4dn.xlarge", name=None)
```

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
