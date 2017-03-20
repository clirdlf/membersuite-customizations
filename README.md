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

## Get a copy

```
$ wget --mirror --convert-links --adjust-extension --page-requisites --no-parent https://customer26007fb00.portal.membersuite.com/Login.aspx
```

## Development Setup

You will need PHP and Ruby to run this project. Ruby dependencies can be installed with `bundle`.

## Development

- Start up the processes (`foreman start`).
- Remove the hard-coded CSS in `customer26007fb00.portal.membersuite.com/Login.aspx.html` (around line 106)
- Link to the css file (`<link href="../css/style.css" />`)
- Open your browser to <http://localhost:8000/customer26007fb00.portal.membersuite.com/Login.aspx.html>
- Edit `_scss/style.css`

### Portal

- Log on to MemberSuite and update the Portal (under **Settings**)
- Copy the contents of `css/style.css` in to the custom CSS field
