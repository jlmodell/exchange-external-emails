# Hide external email warning banner in outlook web/ desktop & mobile

 - Use the below to embed an external email warning banner via an email transport rule
 - [if mso] block targets Outlook desktop
 - Web/Mobile Outlook preheaders do not render styles so we're base64 encoding an SVG banner and setting it as a background of a div.
 - Use this [SVG](https://github.com/jlmodell/exchange-external-emails/blob/main/external-email-warning-banner/warning-banner.svg) to modify the banner & then base64 encode, you can use the following [VS-Code plugin](https://marketplace.visualstudio.com/items?itemName=adamhartford.vscode-base64) to base64 encode.
