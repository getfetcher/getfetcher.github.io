---
layout: post
title:  "Importing Contacts To Fetcher"
date:   2014-1-1
---

Importing contacts from existing platforms can uploaded to fetcher using Commas Separated Files (CSV) or Excel Files. Currently the only three extensions we support are `xls`, `xlsx`, and `csv`. Before attempting to upload a list of contacts, you need to format the columns correct so that our software understands which fields to populate in the contact table. Currently, the only **require** fields for contacts are:

1. primary email (your column should be named primary_email)
1. first name (your column should be named first_name)
1. last name (your column should be named last_name)

The following columns names are currently accepted by GetFetcher.com


1. first_name
1. last_name
1. city
1. state
1. email
1. primary_email
1. full_name
1. affiliation
1. company
1. first
1. last
1. notes
1. title
1. prefix
1. asst_first_name
1. asst_email
1. asst_phone_number
1. mgr_pbl_name
1. mgr_pbl_email
1. partner
1. twitter
1. instagram
1. secondary_email
1. primary_phone
1. secondary_phone

One important thing to notice is we **do not** accept column names with spaces in them: if you want to upload contacts with secondary email addresses, the column name needs to be **secondary_email** not **secondary email**.

Another very important thing to pay attention to is commas when uploading CSV files: CSV files, by definiton, are separated by commas. For GetFetcher.com to successfully upload your file, there needs to be the same number of columns in each row, otherwise that row will be skipped. Therefore, if you have fields with commas in them (such as the affiliation or company fields), you should convert that field to Excel (`xls`,`xlsx`) instead of using CSV so we are  able to successfully upload all of your contacts.