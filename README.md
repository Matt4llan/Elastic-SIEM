# Elastic - SIEM

## Objective

Developing my first dashboard & visualization on Elastic for all failed logon attempts specifically set up to show the Username, Machine ID, Logon Type & Number of records.
I will be adding aditional filters as i go to filter out certain users as a test.

### Skills Learned

- Creating new dashboards and visuals.
- Editing of existing dashboards.
- The use of filters.
- Metrics.

### Tools Used

- Security Information and Event Management (SIEM) Elastic.

## Steps
![image](https://github.com/Matt4llan/Elastic-SIEM/assets/156334555/83831df5-ae01-4e0f-98f9-56217418a9fe)

As we need to create this dashboard with Failed Logon attemtps we need to use filters to achieve this.
The windos code for failed logins is: 4625

![image](https://github.com/Matt4llan/Elastic-SIEM/assets/156334555/885fa518-0f5d-4ae4-898b-e4b6402833c3)

Setting up the visualization as a Table for this example i will start adding in Rows adding in 'user.name.keyword' 'host.hostname.keyword' & 'winlog.logon.type.keyword'
After this we can use the Metric 'Count' to give us a tally

![image](https://github.com/Matt4llan/Elastic-SIEM/assets/156334555/56605e21-a7d3-4faf-b560-33a5b47d56b9)
![image](https://github.com/Matt4llan/Elastic-SIEM/assets/156334555/af3a45c7-6857-451c-a8c9-fec9d7aa885f)

I have renamed the Row headers to make the information more readable and now adding in some Filters to remove some dummy Users from being displayed. This can be used if you have certain test users and anything that you dont want the SIEM dashboard to pick up on.

![image](https://github.com/Matt4llan/Elastic-SIEM/assets/156334555/581d034f-bd2f-4a1d-b3db-afab61229012)

Final mockup of a dashboard showing all failed logon attempts

![image](https://github.com/Matt4llan/Elastic-SIEM/assets/156334555/4f6664b4-d502-4ed3-8da8-020da5568776)



