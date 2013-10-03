This HTML includes a Google Analytics script at the bottom, with some added functions. This functions parse all tags with a "ga-track" class and use the "data-ga" attribute defined in them to specify the term to track.

This way, you can avoid having a onclick="javascript:ga('send', 'event', 'category', 'action', 'label');" on every clickable tag.

The script is kind of long, because a fallback for IE8 and below must be included to get all elements of certain class. When minified, the script is relatively short and it can be included in every HTML with analytics tracking. 
I added a much shorter jQuery version, to be used in jQuery projects.
