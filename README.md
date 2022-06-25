<!-- CREDITS -->
<!-- "Gallery Ahoy!" theme by Alice (DarlingVexa-Art) -->
<!-- Just copy & paste the source code below! This theme is free to use and adjust to suit your needs. -->

<!DOCTYPE html>
<html>
<head>
<style>
/* Link Styles */
a {
    font-family:{titlefont};
    text-decoration: none;
}
/* Link Base */
a:link {
  color: #fff;
  background-color: transparent;
  text-decoration: none;
}
/* Link Visited */
a:visited {
  color: #fff;
  background-color: transparent;
  text-decoration: none;
}
/* Link Hover */
a:hover {
  color: #4aed45;
  text-decoration: none;
}
/* Link Active */
a:active {
  color: #fff;
  background-color: transparent;
  text-decoration: none;
}
/* Paragraph Style */
p {
    margin:5px;
    padding:5px;
}
/* Description Style */
p2 {
    font-family:{titlefont};
    margin:5px;
    padding:5px;
    font-size:15px;
    color:#fff;
}
p3 {
    font-family:{titlefont};
    color:#fff;
}
/* Search Bar Style */
.sfm input {
    font-size: 15px;
    border:0px;
    font-family:{titlefont};
    text-align:left;
    width:{device-width};
    float:left;
}
.sb {
    width:{device-width};
}
/* Header Text/Box Styles */
h3 {
    font-family:{titlefont};
}
h4 {
    font-family:{titlefont};
    margin:5px;
    padding:5px;
    font-size:15px;
    color:#fff;
}
h6 {
    font-family:{titlefont};
    color:{TitleColor};
    height:{description-height};
    font-size:40px;
    margin:5px;
    padding:5px;
}
h7 {
    margin:5px;
    padding:5px;
    color:#fff;
}
/* Navi Style*/
nav {
    background-color:{AccentColor};
    font-family:{titlefont};
    color:{BackgroundColor};
    padding:10px;
    margin:10px;
    text-align:left;
}
/* Search Bar */
subnav {
    background-color:{AccentColor};
    font-family:{titlefont};
    color:{TitleColor};
    height:{description-height};
    width:{device-width};
    padding:11px;
    margin:10px;
    margin-top:-3px;
    float:right;
    text-align:left;
}
/* Body Styles */
body
{
    background-color:{BackgroundColor};
    font-family:{titlefont};
    font-size:15px;
    height:{description-height};
    width:{device-width};
    margin:5px;
    padding:50px;
    text-align:left;
}
body2{
    /* Render on index page */
    {block:indexpage}
    background-color:{AccentColor};
    font-family:{titlefont};
    font-size:15px;
    height:75%;
    margin:10px;
    padding:15px;
    width:21%;
    float:left;
    text-align:center;
    {/block:indexpage}
}
body3{
    /* Render on index page */
    {block:indexpage}
    background-color:{AccentColor};
    font-family:{titlefont};
    font-size:15px;
    height:75%;
    width:70%;
    float:right;
    margin:10px;
    padding:10px;
    text-align:left;
    {/block:indexpage}
    /* Render on custom page */
    {block:custompage}
    font-family:{titlefont};
    font-size:15px;
    height:{Description-Height};
    width:{device-width};
    float:center;
    margin:10px;
    padding:10px;
    text-align:left;
    {/block:custompage}
}
/* Footer Footer*/
footer {
    background-color:{AccentColor};
    font-family:{titlefont};
    color:{BackgroundColor};
    width:{device-width};
    padding:10px;
    margin:10px;
    float:right;
    text-align:left;
}
/* Other Styles */
ol {
    background-color:{AccentColor};
    font-family:{titlefont};
    font-size:15px;
    color:#fff;
    margin:10px;
    padding:10px;
    /* Render on custom pages */
    {block:custompage}
    margin-top:-15px;
    {/block:custompage}
}
ul {
    background-color:{AccentColor};
    font-family:{titlefont};
    font-size:15px;
    color:#fff;
    margin:10px;
    padding:10px;
}
{CustomCSS}
</style></head>

<!-- Background -->
{block:ShowHeaderImage}<body background="{HeaderImage}">{/block:ShowHeaderImage}
<!-- Profile Icon -->
<p>{block:ShowAvatar}<img src="{PortraitURL-128}" width="128px" height="128px" align="center">{/block:ShowAvatar}
</p>
<!-- Username -->
{block:ShowTitle}
<h6>{Title}</h6>
{/block:ShowTitle}
<!-- Description -->
{block:ShowDescription}
<h4>{Description}</h4>
{/block:ShowDescription}
<!-- Assets -->
<link rel="title" href="{TitleFont}">
<link rel="Header" href="{HeaderImage}">
<link rel="Accent Color" href="{AccentColor}">
<link rel="alternate" type="application/rss+xml" href="{RSS}">
<!-- Pages -->
<nav>
<!-- Navigation -->
<a href="{BlogURL}">
Home
</a><p3>|</p3>
<a href="/about">
About Me
</a><p3>|</p3>
<a href="/ask">
Requests
</a><p3>|</p3>
<a href="/info">
Commission Info
</a><p3>|</p3>
<a href="/shop">
Shop
</a><p3>|</p3>
<a href="/archive">
Archive
</a><p3>|</p3>
<a href="/theme">
Theme
</a>
</nav>
<!-- Search Bar -->
<subnav><form action="/search" method="get" class="sfm" width={device-width}>
    <input type="text" name="q" value="{SearchQuery}" id="sf"/>
    <input type="submit" value="Find" id="sb"/>
</form></subnav>
<!-- Quick Tags -->
<h4>
<a href="/search/original">
#original
</a><p3>|</p3>
<a href="/search/oc">
#oc
</a><p3>|</p3>
<a href="/search/fanart">
#fanart
</a><p3>|</p3>
</h4>
<!-- Pagination -->

<!-- Search Results -->
{block:indexpage}
<nav><h4>
    Results for: <u>{SearchQuery}</u><br></h4></nav>
<!-- Featured Image -->
<body2><h4>Featured Image</h4>
<br><a href="{RefreshPage}"><img src="https://64.media.tumblr.com/6c5f68117c86dfd62043c8d1f0e6522b/tumblr_inline_rdr86yF9il1xo4csx_500.png" width="250px" height="250px" border="5px"></a></body2>{/block:indexpage}
<!-- Posts -->
<body3><ol id="posts">
{block:NoSearchResults}
<h4>No results found.</h4>
{/block:NoSearchResults}
<!-- Meta Data -->
{block:Posts}{block:IndexPage}
<a href="{Permalink}">{TimeAgo}</a> | <a href="{PostNotesURL}" target="blank"/>{NoteCountWithLabel}</a> <p3>|</p3> <a href="{BlogURL}">{PostAuthorName}</a><br>{/block:IndexPage}
                <!-- Text Posts -->
                {block:Text}
                        {block:Title}
                            <h3><a href="{Permalink}">{Title}</a></h3>
                        {/block:Title}
                       {Body}{block:HasTags}
                       <ul class="tags">{block:Tags}
                        <a href="{TagURL}">{Tag}</a> <p3>|</p3> 
                        {/block:Tags}
                    </ul><br>
                {/block:HasTags}
<!-- Like Button -->
{LikeButton color="grey"}<br>
<!-- Reblog Button -->
{ReblogButton color="grey"}
{/block:Text}<br>
                <!-- Photo Posts -->
                {block:Photo}
                        {block:Title}
                            <h3><a href="{Permalink}">{Title}</a></h3>
                        {/block:Title}
                       {LinkOpenTag}<img src="{PhotoURL-500}" alt="{PhotoAlt}" border="5px"/>{LinkCloseTag}</div>{block:Caption}
                       <div class="caption">{Caption}
                       {/block:Caption}{Body}
                       {block:HasTags}
                       <ul class="tags">{block:Tags}
                        <a href="{TagURL}">{Tag}</a> <p3>|</p3> 
                        {/block:Tags}
                    </ul><br>
                {/block:HasTags}
<!-- Like Button -->
{LikeButton color="grey"}<br>
<!-- Reblog Button -->
{ReblogButton color="grey"}
{/block:Text}<br>
                       {/block:Photo}
                <!-- Panorama Posts --> 
                {block:Panorama}
                        {block:Title}
                            <h3><a href="{Permalink}">{Title}</a></h3>
                        {/block:Title}
                        {LinkOpenTag}
                            <img src="{PhotoURL-Panorama}" alt="{PhotoAlt}" border="5px"/>
                        {LinkCloseTag}{block:Caption}
                            <div class="caption">{Caption}</div>{/block:Caption}{Body}{block:HasTags}
                       <ul class="tags">{block:Tags}
                        <a href="{TagURL}">{Tag}</a> <p3>|</p3> 
                        {/block:Tags}
                    </ul><br>
                {/block:HasTags}
<!-- Like Button -->
{LikeButton color="grey"}<br>
<!-- Reblog Button -->
{ReblogButton color="grey"}
                      {/block:Panorama}
                <!-- Photoset Posts --> 
                {block:Photoset}
                        {block:Title}
                            <h3><a href="{Permalink}">{Title}</a></h3>
                        {/block:Title}
                        {Photoset-500}{block:Caption}
                            <div class="caption">{Caption}</div>{/block:Caption}{Body}{block:HasTags}
                       <ul class="tags">{block:Tags}
                        <a href="{TagURL}">{Tag}</a> <p3>|</p3> 
                        {/block:Tags}
                    </ul><br>
                {/block:HasTags}
<!-- Like Button -->
{LikeButton color="grey"}<br>
<!-- Reblog Button -->
{ReblogButton color="grey"}
{/block:Text}<br>
                      {/block:Photoset}
                <!-- Quote Posts --> 
                {block:Quote}
                        "{Quote}"
                        {block:Title}
                            <h3><a href="{Permalink}">{Title}</a></h3>
                        {/block:Title}
                        {block:Source}
                            <div class="source">{Source}</div>{/block:Source}{Body}{block:HasTags}
                       <ul class="tags">{block:Tags}
                        <a href="{TagURL}">{Tag}</a> <p3>|</p3> 
                        {/block:Tags}
                    </ul><br>
                {/block:HasTags}
<!-- Like Button -->
{LikeButton color="grey"}<br>
<!-- Reblog Button -->
{ReblogButton color="grey"}
{/block:Text}<br>
                     {/block:Quote}
                <!-- Link Posts --> 
                {block:Link}
                        {block:Title}
                            <h3><a href="{Permalink}">{Title}</a></h3>
                        {/block:Title}
                        <a href="{URL}" class="link" {Target}>{Name}</a>

                        {block:Description}
                            <div class="description">{Description}</div>{/block:Description}{Body}{block:HasTags}
                       <ul class="tags">{block:Tags}
                        <a href="{TagURL}">{Tag}</a> <p3>|</p3> 
                        {/block:Tags}
                    </ul><br>
                {/block:HasTags}
<!-- Like Button -->
{LikeButton color="grey"}<br>
<!-- Reblog Button -->
{ReblogButton color="grey"}
{/block:Text}<br>
<br><br><a href="{PostNotesURL}" target="blank"/>{NoteCountWithLabel}</a>{/block:NoteCount}<br><br>
                       {/block:Link}
                <!-- Chat Posts --> 
                {block:Chat}
                        {block:Title}
                            <h3><a href="{Permalink}">{Title}</a></h3>
                        {/block:Title}
                            {block:Lines}
                                    {block:Label}
                                        <span class="label">{Label}</span>
                                    {/block:Label}{Line}{/block:Lines}{body}
                       {block:HasTags}
                       <ul class="tags">{block:Tags}
                        <a href="{TagURL}">{Tag}</a> <p3>|</p3> 
                        {/block:Tags}
                    </ul><br>
                {/block:HasTags}
<!-- Like Button -->
{LikeButton color="grey"}<br>
<!-- Reblog Button -->
{ReblogButton color="grey"}
{/block:Text}<br>
                          {/block:Chat}
                <!-- Video Posts --> 
                {block:Video}
                        {block:Title}
                         <h3><a href="{Permalink}">{Title}</a></h3>
                        {/block:Title}
                        {Video-500}{block:Caption}
                            <div class="caption">{Caption}</div>{/block:Caption}{body}{block:HasTags}
                       <ul class="tags">{block:Tags}
                        <a href="{TagURL}">{Tag}</a> <p3>|</p3> 
                        {/block:Tags}
                    </ul><br>
                {/block:HasTags}
<!-- Like Button -->
{LikeButton color="grey"}<br>
<!-- Reblog Button -->
{ReblogButton color="grey"}
{/block:Text}<br>
                       {/block:Video}
                <!-- Audio Posts --> 
                {block:Audio}
                        {block:Title}
                            <h3><a href="{Permalink}">{Title}</a></h3>
                        {/block:Title}
                        {AudioEmbed}{block:Caption}
                            <div class="caption">{Caption}</div>{/block:Caption}{body}{block:HasTags}
                       <ul class="tags">{block:Tags}
                        <a href="{TagURL}">{Tag}</a> <p3>|</p3> 
                        {/block:Tags}
                    </ul><br>
                {/block:HasTags}
<!-- Like Button -->
{LikeButton color="grey"}<br>
<!-- Reblog Button -->
{ReblogButton color="grey"}
{/block:Text}
                {/block:Audio}{PostNotes-16}{/block:Posts}<br>
        <br>
        </ol></body3>
<!-- Index Footer -->
        {block:IndexPage}<footer><a href="{RefreshPage}">Back to top</a> | 
        <a href="/page/1">First</a> |
            {block:PreviousPage}
                <a href="{PreviousPage}">&#171; Previous</a>
            {/block:PreviousPage} |<p2>Page {CurrentPage}</p2>| {block:NextPage} <a href="{NextPage}">Next &#187;</a>{/block:NextPage} | <a href="/page/11">Last</a> | <a href="/archive">Archive</a>
        </footer>{/block:IndexPage}
<!-- Misc. Page  -->
{block:CustomPage}
<!-- Misc. Page Footer -->
        <footer>
<a href="{RefreshPage}">Back to top</a> | <a href="{BlogURL}">Home</a> | <a href="/archive">Archive</a> | <a href="/theme">Theme</a>
        </footer>
{/block:CustomPage}
        <!-- End of blog -->
</body>
</html>
