# <img src="../books.svg" alt="Stack of red books with a graduation cap on top, symbolizing education and achievement, set against a plain background" width="30" height="20" /> PL-300 Certification Prep: Microsoft Power BI Data Analyst

## <img src="../notes.svg" alt="Orange pencil lying diagonally on a white sheet of paper, representing note taking and documentation, with a clean and organized appearance" width="20" height="15" /> Part 4 Section 2 - Power BI Pro, Adding Users, and Sharing Reports & Visuals

### Licenses

To read and interact with content others have published to the Power BI service, a Power BI Pro license is required.

### Workspaces

Workspaces contain data sources, semantic models, reports, and dashboards. Create new ones with Workspaces -> New Workspace.

### Creating & Uploading a Report to Power BI Service

#### Slicing Pie Charts

Combining a slicer/legend with a pie chart Can filter down on subcategories if you filter by the category

### Publishing to Power BI

1. Save as
2. Choose a folder
3. Choose a file name
4. Save
5. Go to File
6. Publish
7. Publish to Power BI
8. Select a workspace
9. After publishing, you can go to your workspace and see your uploaded file

### Sharing a Power BI Report

#### Sharing With Users With Free Accounts

1. Share
2. Send link
   - ***People within your organization with this link can view and share***
   - For more options, click the arrow within the “People in your organization with the link can view and share” box
     - Options include people with existing access or specific people
     - You can also either allow recipients of this link to **share the report** or ***allow recipients to build content with the data associated with this report***
     - Click “apply”
3. Enter a name or email address
4. Click send
    - You can also copy the link and send it in an email

### “Permission Required”

`You cannot see the content of this report because you do not have permissions to he underlying dataset`

This error message can also be received by users trying to access a workspace without a Pro license!

### “The Workspaces Shared With Me Are Not Under the Browse -> Shared Tab. Why?”

Items will only appear under the Shared tab if they are shared using the following method:

1. Click “Share”
2. Hovering over the three dots to the right of the “Send Link” header will allow you to manage permissions
   - You can see the folks with access to the link and give direct access
        1. Click the plus sign
        2. Enter a name or email address
        3. Similar options can be given as the previous share method

Browse -> Shared With Me can be a bit temperamental, so it is a good idea to send the link as well. Or, when granting direct access, send an email notification so they have the link regardless.

### Removing Users From Direct Access

Advanced -> Direct Access -> … Remove Reshare or Remove Access (which also removes Reshare)

OR

Power BI tab -> Report - > … -> Manage Permissions -> Click the x

### Sharing Reports and Visuals in PowerPoint

#### Inserting From Power BI

Insert -> Power BI

The Power BI tab will not appear if:

1. You do not have a recent version of PowerPoint
2. You don’t have access to Power BI Pro/Premium
3. Your organizer has disabled this in the Power BI service

#### To Enable Power BI in PowerPoint

Admin portal -> Tenant Settings -> Enable Power BI add-in for PowerPoint (Requires an Administrator)

#### Exporting To PowerPoint

1. Share
2. PowerPoint
3. If you have an existing presentation:
   - Click “Share”
   - Copy the URL Power BI gives you and paste it into your existing presentation
4. If you do not have a presentation:
   - Click “Share”
   - You will receive an “Open in PowerPoint” option

You can also embed an image or live data in PowerPoint!

***NOTE:*** If you have a multi-page report, it will not show in the export.

***If you make changes to the visual or the report, the send link model will have an option to include your changes!***

#### Adding Navigation To PowerPoint

Insert navigation buttons!

1. Click “Buttons”
2. Choose “Navigator” in the Dropdown Menu
   - Click “Page Navigation”
3. If you have an existing presentation:
   - Click “Share”
   - Copy the URL Power BI gives you and paste it into your existing presentation
   - Add a new slide
   - Click “Power BI”
   - Paste URL and click “Insert”
4. If you do not have a presentation:
   - Click “Share”
   - You will receive an “Open in PowerPoint” option

***NOTE:*** You can share individual visualizations similarly to the way you share workspaces!

### Using Reports and Visuals In PowerPoint

Using Presenter Mode, you can interact with a live version of your Power BI workspace! 

**Any changes you make in the edit view will not translate during Presenter Mode, and vice versa!**

#### Embedded Controls

On the bottom right, there are additional options. From left to right:

1. Choosing the bars
   - Filter
     - Hides the filter pane
   - Data insights
     - Provides AI insights
   - Refresh
     - Gets the latest data
   - Reset
2. Choosing the paint brush
   - Adds or removes an outline
   - You can also customize the outline
3. Choosing the blocks
   - Clear the data
   - Get Power BI tips

#### Slide Menu

Can be found on the upper right of the embedded visual or workspace

You can reload, delete it, select it, show it as a saved image (if the original data changes, the image is no longer live)

Showing as a saved image allows you to show folks that don’t have a Power BI account!


## <img src="../question-and-answer.svg" alt="Two speech bubbles, one with a large letter Q and the other with a large letter A, representing a question and answer exchange in a friendly and approachable style" width="35" height="28" /> Cues

- How can you interact with your Power BI report in PowerPoint?
What is the option you see when you click the “...” in the top-right hand corner of the Send Link dialog box?
- To create an interactive report in PowerPoint from Power BI, what do you do after you open the report in the Power BI service?
- How do you share an interactive Power BI report with a person who does not have a paid-for Power BI license?

---

## <img src="../summary.svg" alt="Rolled parchment scroll with visible lines, symbolizing a summary or conclusion, placed on a neutral background" width="30" height="18" /> Summary

Power BI reports can be shared in multiple ways, from directly linking or sharing the report to embedding a live report in Power BI. Using Presenter Mode, you can interact with your embedded report. Any changes you make during Presenter Mode will reset to their original values after the presentation ends.

To create an interactive report in PowerPoint from Power BI, go to “Share”, then click “PowerPoint”, then “Open in PowerPoint”. To share a snapshot of an interactive Power BI report with someone who does not have a paid Power BI license, click on the add-in slide menu and check “Show as Saved Image”. This will show your selected filters on the image (if applicable) and you can save and email the presentation. To make the Power BI report live again, click on the add-in slide menu and un-check “Show as Saved Image”.
