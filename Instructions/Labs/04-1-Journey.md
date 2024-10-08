---
lab:
    title: 'Lab 4.1: Create a trigger-based journey'
---

# Learning Path 4: Create journeys

## Practice Lab 4.1: Create a trigger-based journey 

### Lab Overview

#### Scenario
Now that we have created our 3 emails, it is time to create a journey to send the emails to our customers. We will send our first email to our customers to let them know about the upcoming Airpot Smart Machine Coffee Maker.

Customers that engage with this email will then be split into two sections: customers who already own an old Airpot model, and customers who do not. For our existing Airpot owners, we will send an email encouraging them to upgrade. If they interact with a link on this email, we will have a salesperson reach out to them directly.

Existing owners who did not click a link will get another email advertising the product. This email will also go out to non-Airpot owners.


### What you’ll need:
- A computer with a Dynamics 365 Customer Insights - Journeys environment

## Exercise 1: Create a real-time journey

### Task 1: Create a journey
1.  Log into Dynamics 365 Customer Insights - Journeys.
2.  Navigate to the **Real-time journeys** work area.
3.  Under **Engagement**, select **Journeys.**
4.  Click **+ New journey** in the command bar. If you are prompted to use Copilot to create your journey, select **Skip and create from blank.**
5.  In **Name the journey**, enter *Airpot Smart Machine Launch Campaign.*
6.  In **Choose journey type**, select **Trigger-based.**
7.  In **Choose a trigger**, search for and select **Email Link Clicked.**
8.  In **Choose an email,** search for and select your **Smart Machine Campaign Email.**
9.  Click **Create**.

### Task 2: Configure the journey entry
1. Navigate to the **journey settings** section, which will be expanded on the right side of the screen. The **Entry** section should be open.
2. Leave **Exclude by segments** blank.
3. In the **Repeat** section, select Immediately.
4. In the **Time zone** section, choose your time zone.
5. In **Start,** select today. Set the time to 15 minutes from now. (You can type directly into this field.)
6. In **End,** select tomorrow.

### Task 3: Configure the journey goal
1.  Navigate to the journey settings on the right, which will look like a list of icons. Hover over each icon to see the name of each tab. Select the **Goal** section.
2.  In *The goal of this journey is*, select **Send a general notification.**
3.  In *The goal is met when,* select **A person clicked on at least one link.**
4.  In *The number of people needed,* enter *50.* Leave percent selected.

### Task 4: Add an attribute branch
1. In the journey designer, click the **plus icon (+)** under the **Email link clicked** tile.
2. Select **Attribute branch** from the *Conditions* section.
3. In **Display name** on the right, enter *Already owns airpot*
4. Select **Branch 1**. In Display name, enter *Owns airpot.*
5. Select **Add conditions.**
6. In **Choose an attribute**, Search for **Description (description)** under Contact.
7. Change the value from Equals to Contains.
8. In **Value,** enter *Airpot.*
9. Return to the journey designer. Click the **plus icon (+)** under Branch 1.
  - Select **Email**.
  - In **Select email,** choose **Upgrade Airpot Email.**
10.  Click the **plus icon (+)** under the Send an email tile.
  - Select **Wait for trigger.**
  - In **Choose a branch condition type**, select **The previous message gets an interaction.**
  - In **Choose an interaction**, select **Email Link Clicked.**
  - In **What’s the time limit?,** enter 10 minutes.
11. In the **Yes** path, click the **plus icon (+).**
  - Select **Task** in the Activities section.
  - In Choose a template, select **Follow up with customer.**
  - Subject and Assign to will fill automatically.
  - Change **Due after** to *2 weeks.*
12. In the corresponding **No** path (below the Email Link Clicked If/then branch), click the **plus icon (+).**
  - Select **Send an email**.
  - In **Select email,** choose **Smart Machine Campaign Reminder.**
13. Return to the journey designer. Locate the **Attribute** tile. Now we will configure the **No** branch. For customers that do not already own an Airpot, we will send them the third email.
  - Select the **+** sign under **Other.**
  - Select **Email.**
  - Under Select Email, select **Smart Machine Campaign Reminder.**
14. **Save** the journey.
15. Review the journey. Make any final changes.
16. Click **Publish**. Wait for the journey to publish.
