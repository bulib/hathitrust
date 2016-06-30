# hathitrust
Various python scripts for working with HathiTrust records. 

HathiTrustAnnualReportOfPrintHoldings.ipynb is a python notebook that processes a group of exported records from Alma to produce the annual report of print holdings for submission to HathiTrust. The records are published from a managed set of all print titles. The publishing job embeds item level information in the 949 field. 

For Boston University, a general publishing profile is defined: HT Annual Print Holdings Report

This publishing profile publishes the records in the managed set to an FTP server. As part of the publishing job, the marc_xml records are enhanced with fields from the item records mapped to 949 subfields. The 949 field mapping is below 

#949 field mapping: 
*Material type subfield: k
*Item status subfield: m
*Enumeration A subfield: a
*Enumeration B subfield: b
*Chronology I subfield: c
*Chronology J subfield: d
*Description subfield: e
*Process type subfield: f
*Permanent library subfield: g
*Permanent location subfield: h
*Current library subfield: i 
*Current location subfield: j
