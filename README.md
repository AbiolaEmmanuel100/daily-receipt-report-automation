# Automated Daily Receipt Reporting with n8n & Supabase

**Business Process Automation | n8n | Supabase | JavaScript | HTML Email Reports**

## Project Overview

I built an automated daily reporting workflow for Receipt Pilot, a digital receipt-generation platform. The workflow processes receipt records from Supabase, summarizes daily activity by user, matches users with their business names, and generates a structured HTML report for email delivery.

This project demonstrates how workflow automation can turn raw database records into useful business information without requiring the platform owner to check records manually.

## The Business Problem

Monitoring daily activity across multiple business accounts can become repetitive and time-consuming.

The platform owner needs to know:

* How many receipts were created during the previous day?
* Which users generated those receipts?
* Which businesses are associated with those users?

## My Solution

I used n8n to connect database operations and JavaScript data processing into an automated reporting workflow.

**Workflow process:**

1. Retrieve receipt records from Supabase.
2. Calculate the previous reporting date using the Africa/Lagos timezone.
3. Filter and group receipt records by user.
4. Count the receipts associated with each user.
5. Retrieve business information and match it using user IDs.
6. Generate a formatted HTML report.
7. Deliver the report through email.

## Technology Stack

* **n8n:** Workflow orchestration and automation.
* **Supabase:** Database for receipt records and business information.
* **JavaScript:** Date handling, record processing, grouping, and counting.
* **HTML and CSS:** Report layout and presentation.
* **Email:** Delivery channel for the daily report.

## Testing and Results

During testing, the workflow identified a user who generated nine receipts during the reporting period and displayed the count in the report.

The report was structured around three key fields:

| Field         | Purpose                                            |
| ------------- | -------------------------------------------------- |
| User ID       | Identifies the account associated with the records |
| Business Name | Makes the report easier to interpret               |
| Receipts      | Shows the number of receipts generated             |

## Business Value

This automation provides a practical foundation for monitoring activity across a receipt-generation platform.

Potential benefits include:

* Less repetitive database checking.
* Faster access to daily activity summaries.
* Better visibility into receipt-generation activity across business accounts.
* A reporting process that can be extended as the platform grows.

## Skills Demonstrated

* n8n workflow development.
* Supabase database integration.
* JavaScript data transformation.
* Timezone-aware date processing.
* Grouping and counting business records.
* Matching data across database queries.
* HTML report generation for email.

## Project Scope

**Implemented:** Daily receipt processing, grouping and counting, business-name matching, HTML report generation, and email reporting.

**Not included:** WhatsApp, Telegram, and other messaging integrations.

## Project Screenshots

Screenshots of the n8n workflow and generated email report will be added here.

## Conclusion

This project demonstrates my practical ability to connect a database to an automation workflow, process business data, and produce a structured report that supports day-to-day operations.

It is part of my ongoing development in business process automation and workflow engineering.
