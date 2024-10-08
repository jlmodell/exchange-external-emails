# Hide external email warning banner in outlook web/ desktop & mobile

- EAC > Mail Flows > Rules > New Rule > 'prepend caution for external emails' > 'Is received from `Outside the organization` > 'Prepend the message with the disclaimer' > Except if (optional)

```
Prepend Caution for External Emails
Status: Enabled
Enable or disable rule

Rule settings
Rule name
Prepend Caution for External Emails
Severity
Not specified
Senders address
Matching Header
For rule processing errors
Ignore
Mode
Enforce
Set date range
Specific date range is not set
Priority
0
Rule description
Apply this rule if

Is received from 'Outside the organization'
Do the following

Prepend the message with the disclaimer '<!--[if !mso]><!-->
<div style="background: url('data:image/svg+xml;base64,PHN2ZyBzdHlsZT0id2lkdGg6MTAwJTsiIHZlcnNpb249IjEuMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayIgeG1sbnM6eGh0bWw9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGh0bWwiPg0KICA8c3dpdGNoPg0KICAgIDxmb3JlaWduT2JqZWN0IHg9IjAiIHk9IjAiIHdpZHRoPSIxMDAlIiBoZWlnaHQ9IjEwMCI+DQogICAgICAgICAgICAgIDx4aHRtbDpkaXYgc3R5bGU9ImRpc3BsYXk6aW5saW5lLWJsb2NrO3dpZHRoOjEwMCU7YmFja2dyb3VuZDojZjdlNjhmO2JvcmRlci1sZWZ0OiA4cHggc29saWQgI2ZmYjMwMDt0ZXh0LWFsaWduOmNlbnRlcjtsaW5lLWhlaWdodDoxLjM1O2ZvbnQtc2l6ZToxMXB0O2ZvbnQtZmFtaWx5OiBBcmlhbCwgc2Fucy1zZXJpZjtwYWRkaW5nOjVweCA1cHg7Ym94LXNpemluZzpib3JkZXItYm94OyI+IA0KICAgICAgICAgICAgICAgICAgIDx4aHRtbDpkaXY+ICANCiAgICAgICAgICAgICAgICAgICAgPHhodG1sOnNwYW4gc3R5bGU9ImZvbnQtd2VpZ2h0OmJvbGQ7Ij5DQVVUSU9OOjwveGh0bWw6c3Bhbj4gVGhpcyBlbWFpbCBvcmlnaW5hdGVkIGZyb20gb3V0c2lkZSB0aGUNCiAgICAgICAgICAgICAgICAgICAgb3JnYW5pemF0aW9uLiAgDQogICAgICAgICAgICAgICAgICAgIDwveGh0bWw6ZGl2Pg0KICAgICAgICAgICAgICAgICAgICA8eGh0bWw6ZGl2IHN0eWxlPSJ3b3JkLXdyYXA6IGJyZWFrLXdvcmQ7Ij5EbyBub3QgY2xpY2sgbGlua3Mgb3Igb3BlbiBhdHRhY2htZW50cyB1bmxlc3MNCiAgICAgICAgICAgICAgICAgICAgeW91IHJlY29nbml6ZSB0aGUgc2VuZGVyIGFuZCBrbm93IHRoZSBjb250ZW50IGlzIHNhZmUuDQogICAgICAgICAgICAgICAgICAgIDwveGh0bWw6ZGl2Pg0KICAgICAgICAgICAgICA8L3hodG1sOmRpdj4NCiAgICA8L2ZvcmVpZ25PYmplY3Q+DQogIDwvc3dpdGNoPg0KPC9zdmc+'); height:105px;"></div>
<!--<![endif]-->
<!--[if mso]>
<table border="0" cellspacing="0" cellpadding="0" align="left" width="100%" bgcolor="#f7e68f" style="background:#f7e68f;">
    <tbody>
        <tr style="padding: 5px 0;">
            <td style="background: #ffb300; width:8px;"></td>
            <td style="padding-left:5px;">      
                <div style="line-height: 1.35; font-size: 11pt; font-family: Arial, sans-serif; display:inline-block; width:100%; padding-left:5px; word-wrap: break-word;">
                            <b>CAUTION:</b> This email originated from outside the
                            organization. <br/> 
                            Do not click links or open attachments unless
                            you recognize the sender and know the content is safe.
                  </div>
              </td>
        </tr>
   </tbody>
</table>
<p>&nbsp;</p>

<![endif]-->'. If the disclaimer can't be applied, attach the message to a new disclaimer message.
Except if

Includes these patterns in the From address: '<emails to *whitelist*>'
```
