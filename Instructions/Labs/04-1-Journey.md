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

2.  Navigate to the **Real-time marketing** work area.

3.  Under **Engagement**, select **Journeys.**

4.  Click **+ New journey** in the command bar.
  - If you are prompted to use Copilot to create your journey, select **Skip and create from blank.**
  - In **Name the journey**, enter *Airpot Smart Machine Launch Campaign.*
  - In **Choose journey type**, select **Trigger-based.**
  - In **Choose a trigger**, search for and select **Email Opened.**
  - Click **Create**.

### Task 2: Add elements to the journey
1. From the Journey settings on the right, in the **Entry** section, do the following:
  - Leave **Exclude by segments** blank.
  - In the **Repeat** section, select Immediately.
  - In the **Time zone** section, choose your time zone.
  - In **Start,** select today, 15 minutes from now.
  - In **End,** select tomorrow.

2.  Navigate to the journey settings on the right, which will look like a list of icons. Hover over each icon to see the name of each tab. Select the **Goal** section.
   - In *The goal of this journey is*, select **Send a general notification.**
   - In *The goal is met when,* select **A person clicked on at least one link.**
   - In *The number of people needed,* enter *50.* Leave percent selected.

3.  In the journey designer, click the **plus icon (+)** under the Contact
    Created tile.
  - Select **Attribute branch** from the *Conditions* section.
  - In **Display name** on the right, enter *Already owns airpot*
  - Select **Branch 1**. In Display name, enter *Owns airpot.*
  - Select **Add conditions.**
  - In **Choose an attribute**, Search for **Description (description)** under Contact.
  - Change the value from Equals to Contains.
  - In **Value,** enter *Airpot.*

4.  Return to the journey designer. Click the **plus icon (+)** under Branch 1.
  - Select **Email**.
  - In **Select email,** choose **Upgrade Airpot Email.**

5.  Click the **plus icon (+)** under the Send an email tile.
  - Select **Wait for trigger.**
  - In **Choose a branch condition type**, select **The previous message gets an interaction.**
  - In **Choose an interaction**, select **Email Link Clicked.**
  - In **What’s the time limit?,** enter 10 minutes.

6. In the **Yes** path, click the **plus icon (+).**
  - Select **Task** in the Activities section.
  - In Choose a template, select **Follow up with customer.**
  - Subject and Assign to will fill automatically.
  - Change **Due after** to *2 weeks.*

7. In the corresponding **No** path (below the Email Link Clicked If/then branch), click the **plus icon (+).**
  - Select **Send an email**.
  - In **Select email,** choose **Smart Machine Campaign Reminder.**

8. Return to the journey designer. Locate the **Attribute** tile. Now we will configure the **No** branch. For customers that do not already own an Airpot, we will send them the third email.
  - Select the **+** sign under **Other.**
  - Select **Email.**
  - Under Select Email, select **Smart Machine Campaign Reminder.**

9. **Save** the journey.

10. Review the journey. Make any final changes.

11. Click **Publish**. Wait for the journey to publish.
