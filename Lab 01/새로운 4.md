# Microsoft Copilot Studio

## Lab 0 1 : Create your first copilot in Microsoft

## Copilot Studio

## Hands-on lab step-by-step

```
May 2024
```
```
Microsoft Copilot Studio Workshop
```

## Contents

- Microsoft Copilot Studio
   - Goals for this lab
   - Prerequisites
   - Exercise 1: Sign in to create a Copilot
   - Exercise 2: Take a quick tour of the user interface
   - Exercise 3: Test your copilot
   - Exercise 4: Create your first topic
   - Exercise 5: Publish your copilot to the demo site for testing
   - Terms of Use


## Microsoft Copilot Studio

This lab is subject to the Terms of Use found at the end of this document.

### Goals for this lab

```
After this lab you will be able to:
```
- Create a new chatbot by using the unified authoring canvas in
    Microsoft Copilot Studio.
- Create your first topic and add content to the topic, including rich text
    responses and more.
- Use the **New Copilot** feature in Microsoft Copilot Studio to create a
    topic with AI.
- Learn how to test your bot in Microsoft Copilot Studio.
- Publish your bot on a demo website.^

```
The time to complete
this lab is [ 35 ] minutes.
```
### Prerequisites

Please note that some labs, especially later labs, do reference previous labs in reference to capabilities and previous
tasks. The labs have been designed so as long you have access to a Microsoft Copilot Studio trial. You can get started
from most lab without having to complete the previous module to be able to move forward. However, for the best
experience that shows the features and functionality that is possible within the product, it is recommended you have
completed specific modules before starting some of the labs.

For Lab 01: Create your first copilot in Microsoft Copilot Studio, you need:

- A computer with internet access.
- Be able to log into the provided Microsoft tenant (some companies enforce users to only connect to their
    company tenant).


### Exercise 1: Sign in to create a Copilot

In this exercise, you will use the provided credentials to log into the Microsoft Copilot Studio authoring experience.

Task 1: setup your browser experience

To avoid conflicting with your existing logged-in experiences, you can do these labs by using **one** of these 3 options:

1. **Set up a new work profile** specific to that workshop
    💡 **Pro tip:** _best option to switch between your work and trial environments while keeping history of your work._
    _Ideal if you want to continue using the account later_.
2. Or **browse as a guest**.
3. Or **start an InPrivate session**.


Task 2: log into Copilot Studio

1. Navigate to aka.ms/CopilotStudioStart
2. Enter the provided user name, click **Next**
3. Enter the provided password, click **Sign in**
4. If prompted, choose whether to **stay signed in**.
5. The first time you access Microsoft Copilot Studio, you’ll be prompted to choose your country/region. You
    can choose a value or leave the default option and click **Get Started**.


Task 3 : Create a copilot

1. If you don’t have any existing copilot, you’ll be automatically redirected to the creation experience.
2. Give your copilot a name, **‘{User Prefix} Contoso Customer Service’**
    💡 **Important** : your Copilot’s name must be unique; if an error says it already exists, choose a new prefix
3. Choose the base language of your bot, **English (United States) (en-us)**
    💡 **Pro tip:** _this is the language you will author your copilot in. You can add more languages later_
4. Select **Create**


### Exercise 2: Take a quick tour of the user interface

Microsoft Copilot Studio makes it easier for you to build basic to advanced Copilots. The following section reviews
the main pages of the maker experience for Microsoft Copilot Studio.

Because the Copilot area was explained in the preceding section, the ensuing section will cover the main options that
are available after you select a Copilot.


A. **Overview page** - Displays your home page, including links to test your Copilot, publish your Copilot, and to
documentation.

B. **Topics page** - Where you can view, delete, create, and edit conversation topics.

C. **Generative AI** – Where you can configure settings related to Generative AI, such as configuring data sources,
enabling dynamic chaining, and providing custom instructions.

D. **Actions (preview) page** - Where you can create actions with existing Power Platform components, and
dynamically chain actions together to create automatic responses.

E. **Entities page** - Where you can view and create entities that Microsoft Copilot Studio can recognize in
customer conversations and then load into variables.

F. **Analytics page** - Where you can view metrics to monitor how well your Copilot is serving your customers
and find ways improve it.

G. **Publish page** - Where you can publish the Copilot for team testing or to engage with your customers.

H. **Extend Microsoft Copilot (preview) page** - Where you can extend your Copilots with Microsoft Copilot
through conversational plugins and integrate AIs from the AI Builder.

I. **Settings page** - Where you can select the following different options:

- Copilot details - Change your Copilot's name and image, and get data, such as environment ID, Tenant
    ID, and Bot app ID.
- AI integration tools - Use to extend your Copilot's conversational capabilities.
- Channels - Select one of these options (such as your website or Facebook) that you want customers to
    interact with your Copilot.
- Customer engagement hub - Set up the connecting of Microsoft Copilot Studio to engagement hubs.
- Security - Set up to let your users sign in to their account with you when they're using the Copilot.


### Exercise 3: Test your copilot

1. To show the **Test copilot** pane, in the lower-left corner of the screen, select **Test your copilot**. (If the button
    says **Hide copilot** , then your **Test copilot** pane is already showing.)


2. The **Test copilot** pane shows that a message has already been sent to you from the Copilot. This message
    was sent from the **Conversation Start** topic, which begins automatically. At the **Type your message** prompt,
    at the bottom of the **Test copilot** pane, enter **Hello** and then select the **Send** button.

```
The Copilot will offer a greeting in the Test Copilot pane
```

3. In the **Test copilot** pane, enter **stores near me** as the message and then select the **Send** button. One of the
    prebuilt topics (Lesson 2 Topic) will be triggered in the Copilot, and it will ask you what location you're
    interested in.
4. In the test chat, select the store location that you want. The Copilot will respond with specific information
    based on your selection.

```
Now that you've reviewed an existing topic, you can move on to the next exercise to create a new topic.
```

### Exercise 4: Create your first topic

Task 1: Create a new topic manually

In this first task, you manually create a new topic by following these steps:

1. Select **Topics** in the left menu within Microsoft Copilot Studio.
2. From the **+ Create** drop down at the top of the screen, select **Topic** and then the **From blank** option.
3. Select **Phrases** on the right-hand side of the page underneath **On Recognized Intent properties**

```
(If you’ve closed the On Recognized Intent properties panel , you can click Edit underneath Phrases on the
main Trigger node in the canvas to show the Phrases panel)
```
4. Enter the following phrases, hitting **enter** after each phrase to begin the next one:

```
a. order status
b. track my order
c. where is my package
d. check order status
e. has my order shipped
```

These phrases are added on the right side panel (as shown in the following screenshot). The phrases are also
visible in the Trigger Phrases node.


5. Select the **Details** button within the top right corner to open the Topic Details pane. Rename your topic to
    **Check Order Status** , and then select **Save**.


Task 2: Review the topic UI

Now that you created your first topic, albeit without content except trigger phrases, you can explore the authoring
user interface (UI) to become more familiar with it.


A. **Topic title** - The name of the topic that you're currently creating, which is visible on the Topics page.

B. **Productivity bar** - Where you have access to productivity tools, such as copy and paste, which is available in
Preview.

C. **Comments, Topic checker, and the Test and Save buttons** - This area includes the Topic checker, which
you can run anytime from the authoring canvas to check if errors have occurred in your topic that the
platform can detect, including missing messages in message nodes. Selecting the Test option will open the
Copilot testing panel on the left side of the screen. Selecting the Save icon, which is available when unsaved
changes are present, will save the topic. With the extended menu button (...), you can open the code editor in
Microsoft Copilot Studio preview, allowing users to switch from the graphical view and the code view
seamlessly.

D. **Edit with Copilot, Variables, Analytics, and Details buttons** - The options in this area provide three areas
where you can access all variables that are available in this topic and globally. Selecting Analytics shows key
metrics that are tracked within a time period, including sessions and abandon rate. Selecting the Details
menu allows you to change the name and description of the topic and turn on or turn off the topic.

E. **Properties pane** - This area offers an extended menu item that allows for extra information or control,
depending on what you select. Some items don't have extended options, so this area can be empty on
occasion. Alternatively, by selecting a question node's properties (for example), you have more options to
choose from in this section, such as Question Behavior.

F. **Nodes** - This section shows nodes, which are referred to as the items within an authoring canvas in Microsoft
Copilot Studio. Often, nodes have a type that drives what options are available and required. Examples
include the message node, question node, or topic node.

G. **Authoring canvas** - The area where you'd create your topic. This area is referred to as a canvas due to the
empty space that it gives you to build and connect nodes. It might look empty to begin with, but when you
start adding nodes, such as conditions, the canvas fills up quickly.

H. **Authoring canvas controls** - You can use these controls to navigate the authoring canvas, which can
become large for extensive topics. The included controls are zoom, grab, and selection.


Task 3: Add content to your topic

This exercise doesn't cover how to add a large amount of content to your topic; rather, it provides the steps to add a
single question node, message node, and topic redirection so that you can become familiar with the overall process
of creating a topic, testing, and publishing in Microsoft Copilot Studio. The Publish demo exercise in this module
covers a more in-depth review of the authoring capabilities in Microsoft Copilot Studio.

The next section of this exercise covers foundational knowledge for understanding the central components of
Microsoft Copilot Studio and creating topics.


_Fundamental knowledge: Question node_

As a Copilot author, you should use the Question node when you're expecting a response from the user and you
want to do something based on that information. The user response is stored in a variable, and question nodes can
also use entities and slot filling features, both concepts that are covered later in this exercise.

The Question node uses many functions that a Message node does, such as rich text, speech authoring, and rich text
response types such images, videos, and adaptive cards.

1. In the topic that you have open from the previous task, select the **+ button** below the existing node in the
    canvas and then select **Ask a question** to add a new Question node.
2. Enter **What would you like to do with your order?** in the field and then make sure that the Identify value is
    set to **User's entire response**. This node is asking the question after the topic is triggered about what the
    user wants to do. The Publish demo exercise extends this task to using entities and slot filling.


_Fundamental knowledge: Message node_

You can use the Message node to display a message to the user. This message can be simple based on the topic of
the conversation. In direct contrast to the Question node, the Message node doesn't expect or store an answer from
the user. The Message node has rich text options that you can display in text. You can also use variables within
message nodes in the body of text displayed to the user, which is dynamic based on the data stored within them. This
capability allows messages to be more personal, such as Hello {name}, I can get those order details for you, one
moment. Variables can also store data to perform automation or calculations on them. Later exercises cover variables
more in depth.

1. To add another node, select the **+ button** below the Question node. Then, select **Send a message**. Enter a
    message that acknowledges the customer's question, such as **Thank you for your question!.**


2. End the conversation for the customer in this demo scenario. Select the **+ button** below the message node within
    the authoring canvas. Hover over the **Topic management** option, and then select **End conversation** to end the
    conversation.
3. Then, within the top right hand corner of the screen, select the Save button.


Task 4: Use Copilot in Microsoft Copilot Studio to create a topic

Creating topics in Microsoft Copilot Studio is more effortless than before. Now, you can create a topic in Microsoft
Copilot Studio by using natural language to describe what you want the topic to do. With the Create from description
with Copilot feature, you can automatically build a topic, reducing some manual steps that you experienced from the
first task in this unit. In this task, you'll learn how simple and quick creating a topic with Copilot can be.

1. Select **Topics** from the navigation pane to the left of the screen.
2. Select the **+ Create** drop down and choose **Topic** and then **Create from description with Copilot**. A new
    window appears, asking you to Name your topic and enter a description in the **Create a topic to** space.
3. Enter **Order Status** in the Name your topic field.
4. In the **Create a topic to** space, enter **Create a topic that provides the status of an order for a customer,**
    **asking them their name, order number, and when it was ordered**.
5. Select **Create**.


```
Copilot creates your topic, including the trigger phrases, question nodes, entity selection, variable naming,
and message node confirmation.
```
6. Select the **Edit with Copilot** button in the upper part of the authoring canvas (if the **Edit with Copilot** panel
    isn't open already).
7. Within the **Edit with Copilot** panel, in the field **What do you want to do?,** enter **Ask a question to find out**
    **the user's preferred contact method, choosing from email, phone or SMS**. Then, select Update.


Copilot automatically adds a question node, which both asks the customer for their contact method, and
stores their choice in a variable.


The Copilot feature in Microsoft Copilot Studio drastically reduces authoring time, allowing you to create new topics
and edit topics by using natural language. Additionally, the **Edit with Copilot** panel shows what updates have been
created, and it provides suggestions for what you can update in your topic. Additionally, Copilot in Microsoft Copilot
Studio can create Adaptive Card JSON. Try it by asking Copilot to summarize the information that you've gathered
from the user in an Adaptive Card.

To complete the exercise, **save** this topic. Within the Topics menu in Microsoft Copilot Studio, turn off the topic by
switching the Status toggle to Off, as shown in the following screenshot.


Task 5: Test your Copilot

Now, you will test the Check Order Status topic that you created in the first task.

1. Select the **Test your copilot** button in the lower left corner of the screen to open the testing panel.
2. The **Conversation Start** message appears, and your Copilot starts a conversation. In response, enter a trigger
    phrase for the **Check Order Status** topic that you previously created in the exercise. Remember, after turning
    off the Order Status topic you just created with Copilot, it won't be available in the Test Copilot area.

```
Your message appears, and your Copilot responds as instructed by the topic designed in the previous steps.
Now, the topic is working as it should, and it's time to publish your Copilot.
```

### Exercise 5: Publish your copilot to the demo site for testing

Task 1: Change your bot authentication

For the purposes of this demo, we will set the bot to no authentication so that anyone with a link to the demo site is
able to test it. To do this, follow the below steps:

1. Go to **Settings** in the left-hand navigation
2. Go to **Security** underneath the **Settings** menu
3. Select **Authentication** on the **security** page
4. Select **No authentication** in the panel that opens and select **Save**
5. Select **Save** in the **Save this configuration?** Panel that opens


Task 2: Publish your copilot

Microsoft Copilot Studio provides a demo website so that you can invite anyone to test your Copilot by sending them
the URL. This demo website is useful for gathering feedback to improve your content before you activate the Copilot
for your real customers.

1. In Microsoft Copilot Studio, select the **Publish** page within the navigation pane to the left.
2. Select **Publish** to push the latest topics to the demo website. You'll need to complete this action before you
    use the demo site the first time and after you make changes to the topics that you want people to test on the
    demo website. (When you've created your real Copilot, you'll publish whenever you want to make updated
    topics available to your customers.)
3. Then, select **Publish** again within the publish latest content pop-up dialog.

```
The publishing process checks for errors in the topics whose Status is On. Publication should take only a few
minutes.
```
```
After you've selected the Publish option, a green banner notification will show at the top of the screen when
publishing is complete.
```

4. Select the link for the **demo website** , as shown in the following screenshot.
5. When the demo site window opens, you can interact with the Copilot by typing at the Type your message
    prompt or by selecting a starter phrase from the provided options.

Congratulations, you've now built and published your first Copilot.


### Terms of Use

By using this document, in whole or in part, you agree to the following terms:

**Notice**

Information and views expressed in this document, including (without limitation) URL and other Internet Web site
references, may change without notice. Examples depicted herein, if any, are provided for illustration only and are
fictitious. No real association or connection is intended or should be inferred. This document does not provide you with
any legal rights to any intellectual property in any Microsoft product.

**Use Limitations**

Copying or reproduction, in whole or in part, of this document to any other server or location for further reproduction or
redistribution is expressly prohibited. Microsoft provides you with this document for purposes of obtaining your
suggestions, comments, input, ideas, or know-how, in any form, ("Feedback") and to provide you with a learning
experience. You may use this document only to evaluate its content and provide feedback to Microsoft. You may not use
this document for any other purpose. You may not modify, copy, distribute, transmit, display, perform, reproduce, publish,
license, create derivative works from, transfer, or sell this document or any portion thereof. You may copy and use this
document for your internal, reference purposes only.

**Feedback**

If you give Microsoft any Feedback about this document or the subject matter herein (including, without limitation, any
technology, features, functionality, and/or concepts), you give to Microsoft, without charge, the right to use, share, and
freely commercialize Feedback in any way and for any purpose. You also give third parties, without charge, the right to
use, or interface with, any Microsoft products or services that include the Feedback. You represent and warrant that you
own or otherwise control all rights to such Feedback and that no such Feedback is subject to any third-party rights.

**DISCLAIMERS**

CERTAIN SOFTWARE, TECHNOLOGY, PRODUCTS, FEATURES, AND FUNCTIONALITY (COLLECTIVELY "CONCEPTS"),
INCLUDING POTENTIAL NEW CONCEPTS, REFERENCED IN THIS DOCUMENT ARE IN A SIMULATED ENVIRONMENT
WITHOUT COMPLEX SET-UP OR INSTALLATION AND ARE INTENDED FOR FEEDBACK AND TRAINING PURPOSES
ONLY. THE CONCEPTS REPRESENTED IN THIS DOCUMENT MAY NOT REPRESENT FULL FEATURE CONCEPTS AND MAY
NOT WORK THE WAY A FINAL VERSION MAY WORK. MICROSOFT ALSO MAY NOT RELEASE A FINAL VERSION OF SUCH
CONCEPTS. YOUR EXPERIENCE WITH USING SUCH CONCEPTS IN A PHYSICAL ENVIRONMENT MAY ALSO BE DIFFERENT.

THIS DOCUMENT, AND THE CONCEPTS AND TRAINING PROVIDED HEREIN, IS PROVIDED “AS IS”, WITHOUT WARRANTY
OF ANY KIND, WHETHER EXPRESS, IMPLIED, OR STATUTORY, INCLUDING (WITHOUT LIMITATION) THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, TITLE, AND NONINFRINGEMENT. MICROSOFT DOES NOT
MAKE ANY ASSURANCES OR REPRESENTATIONS WITH REGARD TO THE ACCURACY OF THE RESULTS, THE OUTPUT THAT
DERIVES FROM USE OF THIS DOCUMENT OR THE CONCEPTS, OR THE SUITABILITY OF THE CONCEPTS OR INFORMATION
CONTAINED IN THIS DOCUMENT FOR ANY PURPOSE.

MICROSOFT COPILOT STUDIO (1) IS NOT INTENDED OR MADE AVAILABLE AS A MEDICAL DEVICE FOR THE
DIAGNOSIS OF DISEASE OR OTHER CONDITIONS, OR IN THE CURE, MITIGATION, TREATMENT OR PREVENTION OF
DISEASE, OR OTHERWISE TO BE USED AS A COMPONENT OF ANY CLINICAL OFFERING OR PRODUCT, AND NO LICENSE
OR RIGHT IS GRANTED TO USE MICROSOFT COPILOT STUDIO FOR SUCH PURPOSES, (2) IS NOT DESIGNED OR




