# Mailbox IMAP Flags

Reference for the IMAP flags used by the mailbox.org ecosystem

> **DISCLAIMER** <br> I have no experience with emailing systems. All of my findings are completely superficial and may be incomplete and incorrect.

## IMAP response
The IMAP response itself contains a ```Flags``` and a ```Keyword``` section as in the following sample. These both hold the non IMAP specific flags listed below. In addition the ```Flags``` section also holds general IMAP flags like ```\\Seen``` ```\\Flagged``` etc.
```text
UID	SUBJECT	Flags: ['$cl_0', '$ct_user_0001_3', '\\Seen'] Keywords: ['$cl_0', '$ct_user_0001_3']
```

## Coloured flags

The following IMAP flag identifiers map to the corresponding mailbox flag colours. All of the  identifiers (except no flag) also induce the ```\\Flagged``` flag.

```text
$cl_0   no flag
$cl_1   red
$cl_2   blue
$cl_3   green
$cl_4   gray
$cl_5   purple
$cl_6   light green
$cl_7   orange
$cl_8   pink
$cl_9   cyan
$cl_10  yellow
```

## Predefined mailbox categories

```text
$ct_predefined_0001  Important
$ct_predefined_0002  Business
$ct_predefined_0003  Meeting
$ct_predefined_0004  Private
```

## Custom user categories

```text
$ct_user_0001_3  first created category
$ct_user_0002_3  second created category
$ct_user_0003_3  third created category
...              ...
```

## Thunderbird

Instructions on how to utilize these flags in Thunderbird:

https://kb.mailbox.org/en/private/e-mail/colored-e-mail-flags-for-thunderbird/#flags-in-mailbox-office-and-their-use-in-thunderbird
