# regex-world

Regex everything you see (backup)

##Username

`/^[a-z0-9_-]{3,16}$/` 

Find the start of string(^) and match a string with content `[a-z0-9_-]` and length `{3,16}` and then mark it as the end($)

##Hex value like `#fffd5f` or `#fff`

`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

Easy to understand if you got the last one, `|` means or

##Email

`/^([a-z0-9_\.-]+)@([a-z0-9\.-]+)\.([a-z\.]{2,6})$/`

Also very easy, the `([a-z\.]{2,6})` at the end contains `.` means we should consider both of `.com` and  `.co.cc`

##URL

`/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`

Dame too simple, no description

##HTML Tag

`/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/`

Hard to explain
