## Power BI Deployment Pipelines
-----

- The tool is designed as a pipeline with three stages:

### Development

- This stage is used to design, build, and upload new content with fellow creators. This is the first stage in deployment pipelines.

### Test

- You're ready to enter the test stage after you've made all the needed changes to your content. You upload the modified content so it can be moved to this test stage. Here are three examples of what can be done in the test environment:
- Share content with testers and reviewers
- Load and run tests with larger volumes of data
- Test your app to see how it will look for your end users

### Production

- After testing the content, use the production stage to share the final version of your content with business users across the organization.

### Navigation Steps

1. Click on Workspace **rritec-workspace** > Click on **settings** > Click on Premium > select storage as small blobs > click on **ok**
1. Click on **Deployment Pipelines** > Click on **Create a Pipeline** > Provide pipeline name as **rritecPipeline** >click on **Assign Workspace** > from drop down select **rritec-workspace** > Select **Development** > Click on assign
1. Click on **Deploy** to copy content (Datasets/reports/dashboards) to **Test**
1. Click on Test **Deploy** to copy content from **Test** to **production**
### On going Changes:
1. How to deploy new 1 or couple of reports into other environment?
2. How to deploy Modified report from lower environment to higher environment?
3. How to decommission(Delete) a report?
### Questions
1. After deployment(from dev to test) one report added to dev. Then will it automatically will appear in test?
  - NO, We need click on Dev **Deploy** button
2. As a developer what workspace i will have access?
  - Dev
3. Accidentely removed one report from Dev, Can i copy a report from test to dev?
  - No. (Work around is Request Admin to download PBIX file from test and publis pbix file to Dev)
4. 
