---
lab:
    title: 'Lab 3.2: Create an email'
---

# Learning Path 3: Manage customers and assets in Dynamics 365 Customer Insights - Journeys

## Practice Lab 3.2: Create an email

### Lab Overview

#### Scenario
For this campaign, the marketing team plans to do a large blitz around its newest smart coffee machine. They plan to send a three-email series. The first email will promote Contoso’s Smart Coffee Machine. The second email is intended to encourage customers to fill out a form for more information. The third email is a confirmation email once the form has been submitted.

### Lab Overview
This lab comprises three exercises:
1. In this exercise, you will create an email using an email template.
2. In this exercise, you will create an email by copying another email.
3. In this exercise, you will create an email by copying another email.

### What you’ll need:
- A computer with a Dynamics 365 Customer Insights - Journeys environment

### Exercise 1: Create an email from a template
1. Log into Dynamics 365 Customer Insights - Journeys. Ensure you are in the Real-time marketing area.
2. Navigate to Emails under the Channels group.
3. Click +New to create a new email.
4. From the template gallery, select 1-2 column under Layouts, then click the Select button.
5. In the upper left corner, change the name of the email from Email 1 to Smart Machine Campaign Email.
6. Select the From Name/Subject box in the designer to display the Email header details on the right.
   - Type the following in the Subject: “Finally, a Coffee Machine that gets me”.
   - Make sure that the From name says Contoso Coffee.
7. In the Toolbox, switch to the Theme tab.
   - Note: The details in this section affect the entire email. If you add new text elements to the email, it will default to the font, size, and color listed here. You can then update those elements as needed.
   - Change the Font family to Segoe UI.
   - Change the body text color to: #404040.
   - Change the email background color to #CCCCCC.
8. Select the first section. Change the Section background color to white.
9. Update the logo.
   - Select the image on the designer.
   - On the right, click the placeholder image. Select Replace image then choose Browse library.
   - Select the Contoso logo then click Select.
   - Replace the Alt text with Contoso icon.
   - On the right, click the Link to drop down then select URL then enter www.microsoft.com.
   - In the Size and alignment section, if Auto width is checked, uncheck it. Enter 150px by 50px. Note you may have to click the unlink icon between width and height to set both.
10. Update the image.
   - Select the image in the section below the logo.
   - Select Replace image and Browse library.
   - Select the Hero page image.
11. Select the text section below the logo.
   - Navigate to the section.
   - Change the Section background color to white.
   - Update the header text.
     - Put your cursor at the start of the header text then click the Personalization icon in the toolbar. Select First name from the dropdown. Ensure Contact is selected and select Choose.
     - Add a comma and a space after {{Firstname}}.
     - Change “A short headline goes here” to: “we’ve got you covered.”
     - Highlight the text, make it bold and change the font size to 26.
   - Change “Customize your email...” to “The New Airpot XL Intelligent Coffee Machine is like having your own personal Barista.”
   - Highlight the text and change the font size to 18.
12. Select the two-column section below the text.
   - Navigate to the section. Change the Section background color to white.
   - In the left column, make the following updates:
     - Select Image placeholder. Navigate to the image library and select the machine image.
     - Replace the Alt text with: Smart Coffee Machine.
     - In Link to field, select URL. Enter [https://dynamics.microsoft.com/].
     - In the Size and alignment section, uncheck Auto width. Change the size to 150px by 187px. (Note: Keep link selected to ensure the image maintains proportions.)
   - In the right column under the sub header, make the following updates:
     - Select Image placeholder.
     - Navigate to the image library and select the Barista image.
     - Replace the Alt text with: Barista.
     - In Link to field, select URL. Enter [https://dynamics.microsoft.com/].
     - In the Size and alignment section, uncheck Auto width. Change the size to 150px by 130px. (Note: Keep link selected to ensure the image maintains proportions.)
13. Select the section with the social icons.
   - Navigate to the section. Change the Section background color to white.
14. Select the section with the copyright information.
   - Navigate to the section. Change the Section background color to white.
   - Update the copyright from Company Inc. to Contoso Coffee.
15. Make any other changes as desired.
16. On the toolbar, click Save.
17. Select Preview and test.
   - Click Edit sample data. In the Preview personalization pane, enter the first name of the contact you created. Select the contact to watch the personalization change.
   - Preview the email on all screen sizes.
18. Click Ready to send. Click the notification bar to view the errors. 2 errors should be thrown:
   - Compliance profile
   - Purpose
19. Let's fix these errors and get the email ready for sending.
   - Return to the Design tab.
   - Select the Settings section.
   - Expand Compliance.
   - Select the Contoso Americas compliance profile.
   - Make sure Commercial is selected for Purpose.
20. Click the arrow next to Check content. Run the Accessibility checker to see if there are any other issues within the email. Mitigate any other issues as you see fit.
21. On the toolbar, click Ready to send.

### Exercise 2: Create an email by copying an email
1. Log into Dynamics 365 Customer Insights - Journeys. Ensure you are in the Real-time marketing area.
2. Navigate to Emails under the Channels group.
3. Open the email you created in Exercise 1.
4. In the command bar, click the drop-down arrow next to Save. Choose Save as.
5. In the Quick Create menu on the right, name the email Cross Sell Campaign Email 2.
6. In the Subject field, enter “Are we peaking your interest?”
7. Click Save and Close. A pop-up will appear that says Your changes were saved. Click View record to open the new email. Otherwise, navigate back to Emails and open Cross Sell Campaign Email 2.
8. On the designer, change the header text to: “{{Firstname}}, Coffee your way, at your fingertips.”
9. Change the copy below the header to: “From increasing your online operations to adjusting the setup of your offices, your business needs may have changed considerably this past year. Let's review your policy to ensure you are getting all the coverage you need.”
10. Select the next two-column section. Change the Layout from 2 to 1:2.
    - In the left column, make the following updates:
      - Remove the text.
      - Remove the button.
    - In the right column, make the following updates:
      - Remove the image.
      - Remove BUSINESS INTERRUPTION.
      - Change the text to:
        “It's important to have a partner who understands your business. We are so pleased with our experience at Contoso Insurance. They found us the coverage we needed at a great price.” ‎
        ‎-David P.
        ‎Small Business Owner
      - Change the font size to 16 and italicize.
11. Update the button.
    - Select the button.
    - Change Link to to URL.
    - Enter [https://dynamics.microsoft.com/].
    - Change the Button text to REVIEW MY COVERAGE.
    - Expand Size and alignment. Switch Fit to text to Off. Change the width to 200px.
12. On the toolbar, click Save.
13. Preview the email.
14. Click Check content. Correct any errors if needed.
15. On the toolbar, click Ready to send.

### Exercise 3: Create an email by copying an email
1. Log into Dynamics 365 Customer Insights - Journeys. Ensure you are in the Real-time marketing area.
2. Navigate to Emails under the Channels group.
3. Open the email you created in Exercise 2.
4. In the command bar, click the drop-down arrow next to Save. Choose Save as.
5. In the Quick Create menu on the right, name the email Cross Sell Campaign Email 3.
6. In the Subject field, enter “Thanks for contacting us!”
7. Click Save and Close. A pop-up will appear at the upper right that says Your changes were saved. Click View record to open the new email. Otherwise, navigate to the Emails list and open Cross Sell Campaign Email 3.
8. Change the header text to: “Thanks for contacting us!”
9. Change the copy below the header to:
   - We are excited to review your coverage and see what additional services may benefit your business.
   - An agent will be contacting you shortly to schedule a review of your current coverage.
10. Remove the two-column section.
11. On the toolbar, click Save.
12. Preview the email.
13. Click Check content. Correct any errors if needed.
14. On the toolbar, click Ready to send.

