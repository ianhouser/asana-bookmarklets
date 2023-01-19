# Asana bookmarklets

Drag and drop links below to your browser bookmark bar, then navigate to an Asana page and click the bookmark to make the magic happen.
For details, please see [this forum topic](https://forum.asana.com/t/introduction-to-asana-bookmarklets/184620).

### 1. Expand and Collapse Asana Sidebar
//Working again as of January 2023. Asana changed their CSS structure so this needed to be adjusted to match.

-Toggle expansion to 480px: <a href="javascript:(function(){ var desiredWidth = '480px'; if (document.querySelector('#asana_sidebar').style.width != desiredWidth){document.querySelector('#asana_sidebar').style.width=desiredWidth;document.querySelector('.SidebarResizableContainer-sidebarWrapper').style.flex='0 0 ' + desiredWidth;}else{document.querySelector('#asana_sidebar').style.width='240px'; document.querySelector('.SidebarResizableContainer-sidebarWrapper').style.flex='0 0 240px'}})();">▶Expand Sidebar</a>

Note: If you'd like to customize the width of the expansion, simply change the `480px` in the beginning variable: `var desiredWidth = '480px';` 

Here's the code if you'd like to see and tweak it:
`javascript:(function(){ var desiredWidth = '480px'; if (document.querySelector('#asana_sidebar').style.width != desiredWidth){document.querySelector('#asana_sidebar').style.width=desiredWidth;document.querySelector('.SidebarResizableContainer-sidebarWrapper').style.flex='0 0 ' + desiredWidth;}else{document.querySelector('#asana_sidebar').style.width='240px'; document.querySelector('.SidebarResizableContainer-sidebarWrapper').style.flex='0 0 240px'}})();`

It checks the existing sidebar width and changes it to your desired width if it doesn't match, and changes it to the default width if it does. This results in a toggle of the sidebar width.

--- 2. More to come! Any suggestions let me know: <a href="mailto:ianhouser@gmail.com">ianhouser@gmail.com</a>.
