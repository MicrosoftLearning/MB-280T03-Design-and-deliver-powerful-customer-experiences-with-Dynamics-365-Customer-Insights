---
lab:
  title: 'Lab 3.2: Create an email'
  description: This lab will take approximately 45 minutes to complete.
  duration: 45 minutes
  level: 100
  islab: true
---

# Learning Path 3: Manage customers and assets in Dynamics 365 Customer Insights - Journeys

## Practice Lab 3.2: Create an email

### Lab Overview

#### Scenario
For this campaign, the marketing team plans to do a large blitz around its newest smart coffee machine. They plan to send a three-email series. The first email will promote Contoso’s smart coffee machine. The second email is intended to encourage owners of the regular Airpot to upgrade to the new smart machine. The third email is a reminder about the new product launch. 

This lab will take approximately **45** minutes to complete. 

### Lab Overview
This lab comprises three exercises:
1. In this exercise, you will create an email using an email template.
2. In this exercise, you will create an email by copying another email.
3. In this exercise, you will create an email by copying another email.

### What you’ll need:
- A computer with a Dynamics 365 Customer Insights - Journeys environment

## Exercise 1: Create a marketing email
### Task 1: Create an email from a template
1. Log into Dynamics 365 Customer Insights - Journeys and navigate to the **Real-time journeys area.**
2. Navigate to **Emails** under the Channels group.
3. Select **+New** to create a new email.
4. From the template gallery, scroll down to the **Layouts** section. Select **1-2 column**, then select the **Select** button.
5. In the upper-left corner, select **Email 1** and rename it to `Smart Machine Campaign Email`.
   
   > [!TIP]
   > Hover over **Email 1** to make the text box editable.

6. Select the **From Name/Subject box** in the designer to display the Email header details.
   - Type the following in the Subject: `Finally, a coffee machine that gets me.`
   - Select **Contoso Coffee**(Default brand sender) as the sender (if it is not already). The **From name** and **From email** fields should populate and should be read-only.
7. In the **Toolbox** menu on the right, select the **Theme** tab (paintbrush icon), then configuring the following:
   > [!NOTE]
   > The details in this section affect the entire email. If you add new text elements to the email, it will default to the font, size, and color listed here. You can then update those elements as needed.
   - Change the **Font family** to: Segoe UI
   - Change the **Body text color** color to: #404040.
   - Change the **Email Background** to #CCCCCC.
8. In the email itself, find the first section and select it. An Edit layout tab will appear. Change the **Section background color** to a shade of gray.

## Task 2: Update images
In this task, we will update the logo.

1. Select the image in the first section on the designer.
2. In the right pane, hover over the image and select **Replace**, then select **Browse library**.
3. Select the **Contoso logo**, then select the **Select** button.
4. Enter `Contoso logo` for **Alt text** field.
5. Select the **Link to** to drop down, and then select **URL**. Enter `www.contoso.com`
6. In the **Size and alignment** section, turn off the **Auto width** toggle, then enter `150px` for the width. The height updates automatically.
7. Next, we will update the second image in the email. Select the image in the section below the logo.
8. Select **Replace image** and **Browse library.**
9. Select the **hero-page.jpg** image, then select the **Select** button.

## Task 3: Update a headline using personalization
In this task, we will update a headline to reflect the recipient contact's first name.
1. Locate the Preview Text field below the Subject.
2. Select the **Personalization** icon next to the field, then select **First name** from the dropdown. Ensure **Contact** is selected, then select **Choose.**
3. Add a comma and a space after {{Firstname}}.
4. Select the **Text** block in the designer and change the placeholder text to: “We’ve got your coffee breaks covered.”
5. Highlight the text, make it bold and change the font size to *26.*
6. Change “your email with fonts...” to “The New Airpot XL Intelligent Coffee Machine is like having your own personal barista.”
7. Select all the text and change the font size to *18.*

## Task 4: Design the rest of the email
1. Select the two-column section below the text. Change the Section background color to a shade of blue.
2. In the left column, select the image placeholder, then select **Replace image**. Select **Browse library**, select **coffee-machine.jpg**, then select the **Select** button.
3. Enter `Coffee Machine` for  **Alt text** field.
    > [!NOTE]
    > If the image properties pane does not open automatically, select the image and then select the bottom **image** icon in the **Toolbox** menu on the right.
4. In the **Link to** field, select **URL**, then enter `https://dynamics.microsoft.com/`
5. In the **Size and alignment** section, turn off the **Auto width** toggle, then enter `150px` for the width. The height updates automatically.
6. In the right column under the sub header, select the image placeholder, then select **Replace image**. Select **Browse library**, select **barista.jpg**, then select the **Select** button.
7. Enter `Barista` for **Alt text** field.
8. In the **Link to** field, select **URL**, then enter `https://dynamics.microsoft.com/`
9. Select the section with the social media icons. Change the **Section background color** to a shade of gray.
10. Select the section with the copyright information. Update the copyright from *2022 Company Inc.* to *2024 Contoso Coffee.*
11. Make any other changes as desired. Feel free to be creative and use any design experience you have. What do you find eye-catching when recieving a marketing email?

## Task 5: Save and test the email
1. On the toolbar, select **Save.**
2. Select **Preview and test.**
3. Select **Edit sample data**. In the **Preview personalization pane**, enter the first name of a contact you created, then select the contact to watch the personalization change.
4. Return to the **Preview and test** screen. Preview the email on all screen sizes.
5. Select the dropdown arrow next to **Check content**, then select **Accessibility checker** to to see if there are any other issues within the email. Mitigate any issues as you see fit.
6. On the toolbar, select **Ready to send.**

### Exercise 2: Create an email by copying an email

## Task 1: Create an email to existing customers
1. Log into Dynamics 365 Customer Insights - Journeys. In the bottom-left corner, select **Real-time journeys** from the Change area.
2. Under the Channels group, navigate to **Emails** 
3. Open the email you created in Task 1.
4. In the command bar, select the dropdown arrow next to **Save**, then select **Save as**.
5. In the **Quick Create** pane on the right, set the name to `Upgrade Airpot Email`
6. In the **Subject** field, enter `Is it time for an upgrade?`
7. Select **Save and Close**. A pop-up will appear with the message *Your changes were saved*. Select **View record** to open the new email.
    > [!NOTE]
    > You can also navigate back to **Emails** and open **Upgrade Airpot Email** directly.
8. On the designer, select the header text block and replace the text with `{{Firstname}}, coffee your way, at your fingertips.`
9. Select the text block below the header and replace the text with `Your coffee order is as unique as you are. Time to try our new Airpot Smart Coffee Machine.`
10. Select the two-column section below. In the **Layout** field, change the layout to **1:2**.
    - In the left column, make the following updates:
      - Remove the text.
      - Remove the button.
    - In the right column, make the following updates:
      - Remove the image.
      - Change the text to: `Half-caf Americano, or double shot latte? However you choose to fuel your day, Contoso Coffee has you covered`.
      - Change the font size to 16 and select **Italic**
11. Update the button.
    - Select the button.
    - Select **URL** for **Link to** field
    - Enter https://dynamics.microsoft.com/.
    - Change the Button text to `EXPLORE THE NEW SMART MACHINE`
    - Expand **Size and alignment.** toggle **Fit to text** off, then set the width to `200px`.
12. On the toolbar, select **Save.**
13. Select **Preview and test** to preview the email.
14. Select **Check content** and correct any errors if needed.
15. On the toolbar, select **Ready to send**.

### Task 2: Create a follow-up campaign email
1. Log into Dynamics 365 Customer Insights - Journeys. Ensure you are in the **Real-time journeys** area.
2. Navigate to **Emails** under the Channels group.
3. Open the email you created in Task 1.
4. In the command bar, select the dropdown arrow next to **Save**, then select **Save as**
5. In the Quick Create menu on the right, name the email *Smart Machine Campaign Reminder.*
6. In the Subject field, enter “Have you seen the news?”
7. Select **Save and Close**. A pop-up will appear with the message *Your changes were saved*. Select **View record** to open the new email.
    > [!NOTE]
    > You can also navigate back to **Emails** and open **Smart Machine Campaign     Reminder** directly.
8. On the designer, select the header text block and replace the text with: `The new Airpot Smart Machine: available this fall!`
9. Change the copy below the header to: "Our new Airpot Smart Machine is a new way to make coffee. Learn more about the first-of-its-kind coffee machine today."
10. Remove the two-column section.
11. On the toolbar, select **Save.**
12. Select **Preview and test** to preview the email.
13. Select **Check content** and correct any errors if needed.
14. On the toolbar, select **Ready to send.**

