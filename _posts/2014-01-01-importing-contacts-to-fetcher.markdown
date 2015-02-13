---
layout: post
title:  "Importing Contacts To Fetcher"
date:   2014-1-1
---

Importing contacts from existing platforms can uploaded to fetcher using Commas Separated Files (CSV) or Excel Files. Currently the only three extensions we support are `xls` and `xlsx`. Before attempting to upload a list of contacts, you need to format the columns correct so that our software understands which fields to populate in the contact table. Currently, the only **require** columns for contacts are:

1. primary_email 
1. first_name
1. last_name

Don't worry if all of your data is not formatted correctly -- GetFetcher will let you fix any errors you may have before you upload them, as long as your columns are defined correctly.

The following columns names are currently accepted by GetFetcher.com

1. first_name
1. last_name
1. city
1. state
1. code
1. primary_email
1. full_name
1. affiliations (multiple affiliations are specified using `;`)
1. tags (multiple tags are specified using `;`)
1. code
1. notes
1. title
1. partner
1. twitter
1. instagram
1. linkedin
1. secondary_email
1. primary_phone


One important thing to notice is we **do not** accept column names with spaces in them: if you want to upload contacts with secondary email addresses, the column name needs to be **secondary_email** not **secondary email**. All of your columns should be defined in lower case characters also. Thank you!

Another very important thing to pay attention to is commas when uploading CSV files: CSV files, by definiton, are separated by commas. For GetFetcher.com to successfully upload your file, there needs to be the same number of columns in each row, otherwise that row will be skipped. Therefore, if you have fields with commas in them (such as the affiliation or company fields), you should convert that field to Excel (`xls`,`xlsx`) instead of using CSV so we are  able to successfully upload all of your contacts.

#### Uploading Codes

We strongly recommend you provide the `code` column. Codes are used for email templates and routing for blast in Events Correspondence. Different coded contacts receive different emails when you send a blast.

The following codes are currently accepted by Fetcher (case insensitive)

1. Civilian
1. VIP
1. Client
1. Press

If the code column is not specified, or if you leave the cell blank for certain contacts, all contacts missing codes will be defaulted to `Civilian`.
