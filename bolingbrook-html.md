# Bolingbrook website HTML examples

## Events
Event descriptions are contained in an `<article>` tag, and are structured in such a way that a web scraper can easily retrieve data. For example, we look for datetime information in the `<time>` tag, and location information in the `<div class="location">` tag. 
```html
<article class="fullDisplay B_EV">
    <h1>Bolingbrook Summer Concert Series</h1>
    <time>Wednesday, August 1, 2018 at 7:30 PM<br>
</time>
    <main role="main" class="body">
        <div class="image right">
            <a href="/vertical/Sites/{55EB27CA-CA9F-40A5-A0EF-1E4EEF52F39E}/uploads/BB_Concert_Series(7).jpg"><img src="/vertical/Sites/{55EB27CA-CA9F-40A5-A0EF-1E4EEF52F39E}/uploads/BB_Concert_Series(7)_Web.jpg" style="width:420px;" alt="BB_Concert_Series(7).jpg">
</a>
        </div>
        <p>This week,&nbsp;Kashmir (Led Zepplin Tribute Band) will be performing for the&nbsp;Bolingbrook Summer Concert Series!</p>
        <p>The concert series runs every Wednesday night from 7:30pm - 9pm, located the Performing Art Center.</p>
    </main>
    <div class="location">
        <div class="fieldGrid" xmlns:msxsl="urn:schemas-microsoft-com:xslt" xmlns:vbscript="http://mycompany.com/mynamespace">
            <div class="field inline address adr">
                <h4>Address:</h4>
                <span class="value">
<span class="field inline">
<span class="value property name">Performing Arts Center</span>
                </span>
                <span class="field inline">
<span class="value property street-address">375 W. Briarcliff</span>
                </span>
                <span class="field inline">
<span class="value property city locality">Bolingbrook</span>
                </span>
                <span class="field inline">
<span class="value property state region">IL</span>
                </span>
                <span class="field inline">
<span class="value property zip postal-code">60440</span>
                </span>
                </span>
            </div>
        </div>
    </div>
</article>
```

## News
In contrast, information contained in news `<article>` tags is human-readable, but not structured. Also, some news items contain no text, just images. Example: https://www.bolingbrook.com/index.asp?SEC=28490EF8-B3C9-4503-A4C1-B67E0C2B4B0C&DE=3210A58F-86B8-48CD-8106-3282B5A1B3A4&Type=B_PR
```html
<article class="fullDisplay B_PR">
    <h1>Lion King Auditions 2018</h1>
    <main role="main" class="body">
        <div class="image right">
            <a target="" style="width:420px;" href="https://www.facebook.com/events/387851575072682/"><img src="/vertical/Sites/{55EB27CA-CA9F-40A5-A0EF-1E4EEF52F39E}/uploads/lions_audition_Web.jpg" style="width:420px;" alt="For more information on this event, click the image">
</a>
            <div class="small imageBoxCaption" style="width:420px;">For more information on this event, click the image</div>
        </div>
        <p><span>Disney's The Lion King has captivated the imagination of audiences around the world and now, for the first time ever, the African savannah comes to life on our stage with Simba, Rafiki and an unforgettable cast of characters as they journey from Pride Rock to the jungle... and back again, in this inspiring, coming-of-age tale.</span><br><br><span>WHO: Large cast of students grades 2-9</span><br><span>WHEN: Tuesday August 21 5:00 - 7:00 PM</span><br><span>Thursday August 23 5:00 - 7:00 PM</span><br><span>WHERE: Bolingbrook Performing Arts Center,&nbsp;</span><br><span>375 West Briarcliff, Bolingbrook IL</span><br><span>behind Village Center</span><br><span>WHAT: Please come prepared to read, learn a dance, and sing a&nbsp;</span>Capella
            an excerpt from a song of your choice.&nbsp;</p>
    </main>
</article>
```