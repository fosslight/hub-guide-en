---
sort: 5
published: true
---

# OSS Table Warning Message
You can identify issues that need review through the Warning Message in the OSS Table.

## Meaning of Warning Messages by Color
- <span style="color:red"> Red </span>: Needs correction; review request or confirmation is not possible. Review and modify as necessary.
- <span style="color:blue"> Blue </span>: Review request and confirmation are possible, but further review is required. Please check carefully.
- <span style="color:grey"> Gray </span>: Informational message; no specific action is needed.

## Review Items According to Warning Messages

| Message  | Description |
| ------------- | ------------- |
|**This field is required**| This field requires input. |
|**Unconfirmed open source**| This is a new OSS that has not been registered. |
|**Unconfirmed version**| This is a new version that has not been registered. |
|**Unconfirmed license**| This is a new license that has not been registered. |
|**Dual license: Select a license**| It is marked as Dual License, but all licenses are being used. <br>Please select only the licenses you intend to use. |
|**Specify OSS Name or put 1 license in a row**| The OSS Name is either "-" or blank while multiple licenses are written in a single row. <br>If the OSS Name is "-" or blank, please separate the licenses into different rows. |
|**The address should be started with www**| The address format is incorrect. |
|**Formatting error**| Line break characters are included. If multiple lines are needed, please add more rows. |
|**Not the same as property**| The entered URL differs from the URL registered for the corresponding OSS in FOSSLight Hub. |


{% include list.liquid all=true %}
