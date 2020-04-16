[![Author](https://img.shields.io/badge/author-S%C3%A1ndor%20Jablonczay-lightgrey.svg?colorB=9900cc )](https://jablonczay.com/)
[![Twitter](https://img.shields.io/twitter/url/https/github.com/jablonczay/code-box-copy.svg?style=social)](https://twitter.com/jablonczay)

# GDPR Cookie Law – jQuery GDPR Compliance Plugin – Documentation

### What is this?

GDPR Cookie Law is a super fast jQuery plugin that allows you to create simple cookie notification with several options.

#### :link: Demo: [Usage Examples](https://jablonczay.com/gdpr-cookie-law-jquery-gdpr-compliance-plugin/)
#### :link: Purchase: [Buy this GDPR plugin on CodeCanyon](https://1.envato.market/50vqn)

## Quick Start

1. Copy the gdpr-cookie-law folder to your server's document root folder, next to your index.html file. The gdpr-cookie-law folder contains the css and js folders.

2. Add the GDPR Cookie Law CSS files to the head section on your page:

```html
<link rel="stylesheet" href="http://your-domain.com/gdpr-cookie-law/css/gdpr-cookie-law.min.css">
```
3. Add the GDPR Cookie Law JavaScript files to the head or the body section on your page:

```html
<script src="http://your-domain.com/gdpr-cookie-law/js/jquery-3.3.1.min.js"></script>
<script src="http://your-domain.com/gdpr-cookie-law/js/gdpr-cookie-law.min.js"></script>
<script>
$(document).ready(function () {
    $(document).gdprCookieLaw({
        moreLinkHref: 'http://your-domain.com/privacy-policy'
    });
});
</script>
```

4. Set the parameters as you need.


## Parameters

| Property | Possible Values | Default Value | Description |
| --- | --- | --- | --- |
| expire | e.g. 30, 365, 1000, etc. | 365 | The expiration date of the cookie is from the date specified in days. |
| breakpoint | e.g. '768px', '992px', '48em', etc. | '768px' | The width above which the box is aligned vertically. |
| zIndex | e.g. null, '1000', '1111111111', etc. | '1000000000' | The z-index of the box. |
| delay | e.g. null, 500, 1000, etc. | null | The box appears after the specified time (milliseconds). |
| theme | e.g. null, 'theme-dark', 'theme-light', 'theme-1', 'theme-2', ... 'theme-10', and 'theme-light-1', 'theme-light-2' ... 'theme-light-10', etc. | null | The theme of the box. If you set a theme the following options do not apply: background color, background color opacity and the font color of the box, the 'More information' link font color, background color and font color of the accept button (included the hover, focus and active states). |
| animationStatus | true, false | true | The animation status of the box. |
| animationDuration | e.g. 500, 1000, etc. | 500 | The duration time of the animation in milliseconds. |
| animationName | null, 'fade', 'slide', 'fade-slide' | 'fade' | The type of the animation. |
| position | 'bottom', 'bottom-left', 'bottom-center', 'bottom-right', 'top', 'top-left', 'top-center', 'top-right' | 'bottom' | The position of the box. |
| margin | e.g. null, '10px', '20px', '30px', etc. | null | The margin of the box. |
| padding | e.g. '10px', '20px', '30px', '20px 30px', etc. | '20px' | The padding of the box. |
| width | e.g. null, 'auto', '400px', '500px', etc. | 'auto' | The width of the box. It is recommended to use it when top-left | top-right | bottom-left | bottom-right position is specified. |
| bgColor | e.g. '#454545', '#369', '#000', '#fff', etc. | '#09a0e1' | The background color of the box. |
| bgColorOpacity | e.g. 0.5, 0.6, 0.85, etc. | 1 | The transparency of the background color of the box. |
| boxShadowStatus | true, false | true | The shadow's status of the box. If the value is true, the shadow appears. If the value is false, the shadow does not appear. |
| boxShadowHorizontalOffset | e.g. '0px', '10px', etc. | '0px' | The horizontal offset of the shadow. |
| boxShadowVerticalOffset | e.g. '0px', '10px', etc. | '0px' | The vertical offset of the shadow. |
| boxShadowBlur | e.g. '5px', '10px', '30px', etc. | '30px' | The blur of the shadow. |
| boxShadowSpread | e.g. '0px', '10px', '30px', etc. | '0px' | The spread of the shadow. |
| boxShadowColor | e.g. '#000', '#454545', etc. | '#000' | The color of the shadow. |
| boxShadowOpacity | e.g. 0.05, 0.5, 0.8, 1, etc. | 0.05 | The transparency of the shadow. |
| fontFamily | e.g. null, 'Arial, sans-serif', '"Times New Roman", serif' etc. | null | The font family of the box. |
| fontSize | null, '13px', '14px', '16px', etc. | '16px' | The font size of the box. |
| fontWeight | e.g. 'normal', 'bold', 'lighter', 'bolder', '100', '900', etc. | 'normal' | The font weight of the box. Possible values &#8203;&#8203;may vary by font family. |
| color | e.g. '#333', '#369', '#454545', '#fff', etc. | '#fff' | The font color of the box. |
| contentWidth | e.g. null, 'auto', '1170px', '1200px', etc. | 'auto' | The width of the box's contents. |
| contentAndBtnHorizontalSpace | e.g. '32px', '48px', '3em', etc. | '3em' | The horizontal space between the description and the button. |
| contentAndBtnVerticalSpace | e.g. '16px', '32px', '2em', etc. | '2em' | The vertical space between the description and the button. |
| desc | 'Any text what you want' | 'We use cookies to ensure that we give you the best experience on our website. By continuing to use our site, you accept our cookie policy.' | The description of the box. |
| customAnchors | e.g. [ { id: 'cookies', href: 'http://your-domain.com/cookies', title: 'About cookies', target: '_blank', text: 'cookies' }, { id: 'cookiePolicy', href: 'http://your-domain.com/privacy-policy', title: 'Cookie policy', target: '_blank', text: 'cookie policy' } ] | null | You can add custom anchors to the description. E.g. desc: 'We use {{cookies}} to ensure that we give you the best experience on our website. By continuing to use our site, you accept our {{cookiePolicy}}.' |
| moreLinkStatus | true, false | true | The status of the 'More information' link. If the value is true, the 'More information' link appears. If the value is false, the 'More information' link does not appear. |
| moreLinkDecorationStatus | true, false | true | The decoration's status of the 'More information' link. If the value is true, the decoration appears. If the value is false, the decoration does not appear. |
| moreLinkDecorationType | 'none', 'dotted', 'dashed', 'solid' | 'dotted' | The decoration type of the 'More information' link. |
| moreLinkText | 'Any text what you want' | 'More information' | The text of the 'More information' link. |
| moreLinkColor | e.g. '#333', '#369', '#454545', '#fff', etc. | '#fff' | The font color of the 'More information' link. |
| moreLinkFontFamily | e.g. null, 'Arial, sans-serif', '"Times New Roman", serif' etc. | null | The font family of the 'More information' link. |
| moreLinkFontSize | null, '13px', '14px', '16px', etc. | '16px' | The font size of the 'More information' link. |
| moreLinkFontWeight | e.g. 'normal', 'bold', 'lighter', 'bolder', '100', '900', etc. | 'bold' | The font weight of the 'More information' Link. Possible values &#8203;&#8203;may vary by font family. |
| moreLinkHref | URL e.g. 'http://your-domain.com/privacy-policy' | null | The href attribute of the 'More information' link. |
| btnAcceptText | 'Any text what you want' | 'Accept' | The text of the accept button. |
| btnAcceptPaddingTop | e.g. '10px', '12px', '15px' etc. | '15px' | The top padding of the accept button. |
| btnAcceptPaddingRight | e.g. '48px', '52px', '56px', etc. | '56px' | The right padding of the accept button. |
| btnAcceptPaddingBottom | e.g. '10px', '12px', '13px' etc. | '13px' | The bottom padding of the accept button. |
| btnAcceptPaddingLeft | e.g. '48px', '52px', '56px', etc. | '56px' | The left padding of the accept button. |
| btnAcceptBgColor | e.g. '#333', '#369', '#454545', '#fff', etc. | '#0780c0' | The background color of the accept button. |
| btnAcceptBgColorHover | e.g. '#333', '#369', '#454545', '#fff', etc. | '#0670b0' | The hover background color of the accept button. |
| btnAcceptBgColorFocus | e.g. '#333', '#369', '#454545', '#fff', etc. | '#0670b0' | The focus background color of the accept button. |
| btnAcceptBgColorActive | e.g. '#333', '#369', '#454545', '#fff', etc. | '#0670b0' | The active background color of the accept button. |
| btnAcceptColor | e.g. '#333', '#369', '#454545', '#fff', etc. | '#fff' | The font color of the accept button. |
| btnAcceptColorHover | e.g. '#333', '#369', '#454545', '#fff', etc. | '#fff' | The hover font color of the accept button. |
| btnAcceptColorFocus | e.g. '#333', '#369', '#454545', '#fff', etc. | '#fff' | The focus font color of the accept button. |
| btnAcceptColorActive | e.g. '#333', '#369', '#454545', '#fff', etc. | '#fff' | The active font color of the accept button. |
| btnAcceptBorderRadius | e.g. null, '3px', '4px', '10px', '999px', etc. | '999px' | The radius of border for the button. |
| btnAcceptFontFamily | e.g. null, 'Arial, sans-serif', '"Times New Roman", serif' etc. | null | The font family of the accept button. |
| btnAcceptFontSize | null, '13px', '14px', '16px', etc. | '14px' | The font size of the accept button. |
| btnAcceptFontWeight | e.g. 'normal', 'bold', 'lighter', 'bolder', '100', '900', etc. | 'bold' | The font weight of the accept button. Possible values &#8203;&#8203;may vary by font family. |

## Other Projects

- [Elegant Elements – jQuery HTML Form Plugin](https://1.envato.market/j695n)
- [Elegant Age Verification – Responsive age-gate plugin for WordPress](https://1.envato.market/ag5YM)
- [AudioJungle – Royalty free sounds](https://audiojungle.net/user/jablonczay/portfolio)
- [Responsive Testimonals for jQuery](https://github.com/jablonczay/responsive-testimonals-for-jquery/)
- [Scroll Styler – Free Wordpress Plugin](https://wordpress.org/plugins/scroll-styler/)
- [Royalty-free Photos](https://www.shutterstock.com/g/jablonczay)
