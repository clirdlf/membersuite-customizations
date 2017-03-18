# Membersuite Customizations

This is based off the base skin <http://community.membersuite.com/membersuite/topics/custom-menu-or-html> for MemberSuite with customizations.

In case something goes wrong, the default template is this:

```
<div id="siteWrapper">
        <div id="siteWrapperTop">
            <div id="siteWrapperBottom">
                <div id="siteWrapperMiddle">
                    <div id="siteWrapperTopMiddle">
                        <!-- site container -->
                        <div id="siteContainer">
                            <!-- site header -->
                            <div id="siteHeader">
                                <div id="siteHeaderContent">
                                    <a href="{homepageurl}">
                                        <img src="{imageurl}" alt="Header Banner" /></a>
                                </div>
                            </div>
                            $$CONTENT$$
                        </div>
                        <!-- / site container -->
                    </div>
                </div>
            </div>
        </div>
    </div>
```


## Testing the CSS

```
$ sass --watch _scss/style.scss:css/style.css --style compressed
```

```
$ php -S localhost:8000
```
