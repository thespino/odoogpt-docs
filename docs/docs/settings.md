# OdooGPT & OpenAI Settings

All setting can be found at `Settings → Odoo GPT`. 

![Odoo GPT Settings](./settings/settings.png)


## OpenAI Api token

The OpenAI Api Token is required to allow Odoo to communicate with OpenAI apis. 

To get or generate your Api token, go to 
**[OpenAI Dashboard](https://platform.openai.com/account/api-keys){:target="_blank"}**: 

![OpenAI Api Key in dashboard](./getting-started/openai-api-key.png)

Paste the Token in OdooGPT setting in "**OpenAI Api token**" field: 

![OpenAI Api Key in OdooGPT settings](./getting-started/odoogpt-api-key.png)

Save settings.

Then, click on `TEST` button. If you receive the notification 

> Test success! Everything properly set up! You're good to go! 

it means everything is correctly configured.


## OpenAI Model

You can customize the **Model** to use with OdooGPT. This allows also to use custom fine-tuned 
models. Simply write the model name in the field (if you exactly know it) or press `PICK MODEL` 
button to open the table with all the Models read from OpenAI api. 

Default is `text-davinci-003`, which is GPT-3 model.

![OpenAI Model](./settings/model.png)


## OpenAI Parameters

In this section, alongside with the OpenAI Model, you can also find some parameters that allows to 
customize the behaviour of OpenAI. Please refer to 
[OpenAI documentation](https://platform.openai.com/docs/api-reference/completions/create){:target="_blank"} to learn more. 
You can find default valuse in the picture below. 

![OpenAI Parameters](./settings/parameters.png)

!!! info
    Default value for Max Tokens is deliberately low, in order to prevent high usage when in test 
    phase. Recommended value for useful responses is at aound 400 ~ 500 tokens. Please keep that 
    in mind in order to prevent unwanted costs with OpenAI Api. 


## OdooGPT Chat Customization

The following parameters allow to add context to ALL Api requests, in order to allow ChatGPT to 
better understand what you're asking. 

For example, an input of "How to create a Product?" won't give useful answers. But if you prefix it 
with "In Odoo: ", the AI can correctly scope the question because you're adding context. 
Want to be more precise? You could even change it to "In Odoo 16: ". 

The same can be done with a suffix, if needed. 

![OdooGPT Chat Customization](./settings/customization.png)
