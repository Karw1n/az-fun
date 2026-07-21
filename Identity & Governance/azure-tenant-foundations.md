# Creating a pipeline with Azure Data Factory

## Objective
As I was planning out my first project I realised that my tenant has no structure, no subscription, no security groups, no resource groups etc. 

## Steps I took
1. Logon the Azure Portal
2. Navigated to subscriptions on the home dashboard
3. Created a subscription, left most settings as default
4. Decided to create a budget (subscription -> cost management -> budgets ) as I am cautious of building up cost as I'm on the pay-as-you go plan. Budget alerts will inform me If I'm spending any money. My budget tells me if I've spent a pound.
5. I then created a resource group, here you would start to segment depending on the usecase, e.g. if it's a finance resource. In this case it was called "rg-personalproject-test-uksoutch".
6. I attached a tag to indicate it's part of my personal projects.


## Screenshot


## What I learned
Naming resources follow a structure {prefix}-{workload}-{environment}-{region}.
rg: The prefix for Resource Groups.
{workload}: The application or service name (e.g., coreapi, finance, web).
{environment}: The deployment tier (e.g., dev, test, qa, prod, dr).
{region}: The Azure deployment location in short-form (e.g., uksouth, westeurope, useast)

## Gotchas
Alert Recipients in budgets needed to be a unique email address, I couldn't just put in my standard one. It had to be my user principal name which I found in user basic info.