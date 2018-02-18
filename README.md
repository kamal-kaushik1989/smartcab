<!DOCTYPE html>
<html>
<head><meta charset="utf-8" />
<title>smartcab</title><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.0.3/jquery.min.js"></script>

<style type="text/css">
    /*!
*
* Twitter Bootstrap
*
*/
/*!
 * Bootstrap v3.3.7 (http://getbootstrap.com)
 * Copyright 2011-2016 Twitter, Inc.
 * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
 */
/*! normalize.css v3.0.3 | MIT License | github.com/necolas/normalize.css */
html {
  font-family: sans-serif;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
}
body {
  margin: 0;
}
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
main,
menu,
nav,
section,
summary {
  display: block;
}
audio,
canvas,
progress,
video {
  display: inline-block;
  vertical-align: baseline;
}
audio:not([controls]) {
  display: none;
  height: 0;
}
[hidden],
template {
  display: none;
}
a {
  background-color: transparent;
}
a:active,
a:hover {
  outline: 0;
}
abbr[title] {
  border-bottom: 1px dotted;
}
b,
strong {
  font-weight: bold;
}
dfn {
  font-style: italic;
}
h1 {
  font-size: 2em;
  margin: 0.67em 0;
}
mark {
  background: #ff0;
  color: #000;
}
small {
  font-size: 80%;
}
sub,
sup {
  font-size: 75%;
  line-height: 0;
  position: relative;
  vertical-align: baseline;
}
sup {
  top: -0.5em;
}
sub {
  bottom: -0.25em;
}
img {
  border: 0;
}
svg:not(:root) {
  overflow: hidden;
}
figure {
  margin: 1em 40px;
}
hr {
  box-sizing: content-box;
  height: 0;
}
pre {
  overflow: auto;
}
code,
kbd,
pre,
samp {
  font-family: monospace, monospace;
  font-size: 1em;
}
button,
input,
optgroup,
select,
textarea {
  color: inherit;
  font: inherit;
  margin: 0;
}
button {
  overflow: visible;
}
button,
select {
  text-transform: none;
}
button,
html input[type="button"],
input[type="reset"],
input[type="submit"] {
  -webkit-appearance: button;
  cursor: pointer;
}
button[disabled],
html input[disabled] {
  cursor: default;
}
button::-moz-focus-inner,
input::-moz-focus-inner {
  border: 0;
  padding: 0;
}
input {
  line-height: normal;
}
input[type="checkbox"],
input[type="radio"] {
  box-sizing: border-box;
  padding: 0;
}
input[type="number"]::-webkit-inner-spin-button,
input[type="number"]::-webkit-outer-spin-button {
  height: auto;
}
input[type="search"] {
  -webkit-appearance: textfield;
  box-sizing: content-box;
}
input[type="search"]::-webkit-search-cancel-button,
input[type="search"]::-webkit-search-decoration {
  -webkit-appearance: none;
}
fieldset {
  border: 1px solid #c0c0c0;
  margin: 0 2px;
  padding: 0.35em 0.625em 0.75em;
}
legend {
  border: 0;
  padding: 0;
}
textarea {
  overflow: auto;
}
optgroup {
  font-weight: bold;
}
table {
  border-collapse: collapse;
  border-spacing: 0;
}
td,
th {
  padding: 0;
}
/*! Source: https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css */
@media print {
  *,
  *:before,
  *:after {
    background: transparent !important;
    color: #000 !important;
    box-shadow: none !important;
    text-shadow: none !important;
  }
  a,
  a:visited {
    text-decoration: underline;
  }
  a[href]:after {
    content: " (" attr(href) ")";
  }
  abbr[title]:after {
    content: " (" attr(title) ")";
  }
  a[href^="#"]:after,
  a[href^="javascript:"]:after {
    content: "";
  }
  pre,
  blockquote {
    border: 1px solid #999;
    page-break-inside: avoid;
  }
  thead {
    display: table-header-group;
  }
  tr,
  img {
    page-break-inside: avoid;
  }
  img {
    max-width: 100% !important;
  }
  p,
  h2,
  h3 {
    orphans: 3;
    widows: 3;
  }
  h2,
  h3 {
    page-break-after: avoid;
  }
  .navbar {
    display: none;
  }
  .btn > .caret,
  .dropup > .btn > .caret {
    border-top-color: #000 !important;
  }
  .label {
    border: 1px solid #000;
  }
  .table {
    border-collapse: collapse !important;
  }
  .table td,
  .table th {
    background-color: #fff !important;
  }
  .table-bordered th,
  .table-bordered td {
    border: 1px solid #ddd !important;
  }
}
@font-face {
  font-family: 'Glyphicons Halflings';
  src: url('../components/bootstrap/fonts/glyphicons-halflings-regular.eot');
  src: url('../components/bootstrap/fonts/glyphicons-halflings-regular.eot?#iefix') format('embedded-opentype'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.woff2') format('woff2'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.woff') format('woff'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.ttf') format('truetype'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.svg#glyphicons_halflingsregular') format('svg');
}
.glyphicon {
  position: relative;
  top: 1px;
  display: inline-block;
  font-family: 'Glyphicons Halflings';
  font-style: normal;
  font-weight: normal;
  line-height: 1;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.glyphicon-asterisk:before {
  content: "\002a";
}
.glyphicon-plus:before {
  content: "\002b";
}
.glyphicon-euro:before,
.glyphicon-eur:before {
  content: "\20ac";
}
.glyphicon-minus:before {
  content: "\2212";
}
.glyphicon-cloud:before {
  content: "\2601";
}
.glyphicon-envelope:before {
  content: "\2709";
}
.glyphicon-pencil:before {
  content: "\270f";
}
.glyphicon-glass:before {
  content: "\e001";
}
.glyphicon-music:before {
  content: "\e002";
}
.glyphicon-search:before {
  content: "\e003";
}
.glyphicon-heart:before {
  content: "\e005";
}
.glyphicon-star:before {
  content: "\e006";
}
.glyphicon-star-empty:before {
  content: "\e007";
}
.glyphicon-user:before {
  content: "\e008";
}
.glyphicon-film:before {
  content: "\e009";
}
.glyphicon-th-large:before {
  content: "\e010";
}
.glyphicon-th:before {
  content: "\e011";
}
.glyphicon-th-list:before {
  content: "\e012";
}
.glyphicon-ok:before {
  content: "\e013";
}
.glyphicon-remove:before {
  content: "\e014";
}
.glyphicon-zoom-in:before {
  content: "\e015";
}
.glyphicon-zoom-out:before {
  content: "\e016";
}
.glyphicon-off:before {
  content: "\e017";
}
.glyphicon-signal:before {
  content: "\e018";
}
.glyphicon-cog:before {
  content: "\e019";
}
.glyphicon-trash:before {
  content: "\e020";
}
.glyphicon-home:before {
  content: "\e021";
}
.glyphicon-file:before {
  content: "\e022";
}
.glyphicon-time:before {
  content: "\e023";
}
.glyphicon-road:before {
  content: "\e024";
}
.glyphicon-download-alt:before {
  content: "\e025";
}
.glyphicon-download:before {
  content: "\e026";
}
.glyphicon-upload:before {
  content: "\e027";
}
.glyphicon-inbox:before {
  content: "\e028";
}
.glyphicon-play-circle:before {
  content: "\e029";
}
.glyphicon-repeat:before {
  content: "\e030";
}
.glyphicon-refresh:before {
  content: "\e031";
}
.glyphicon-list-alt:before {
  content: "\e032";
}
.glyphicon-lock:before {
  content: "\e033";
}
.glyphicon-flag:before {
  content: "\e034";
}
.glyphicon-headphones:before {
  content: "\e035";
}
.glyphicon-volume-off:before {
  content: "\e036";
}
.glyphicon-volume-down:before {
  content: "\e037";
}
.glyphicon-volume-up:before {
  content: "\e038";
}
.glyphicon-qrcode:before {
  content: "\e039";
}
.glyphicon-barcode:before {
  content: "\e040";
}
.glyphicon-tag:before {
  content: "\e041";
}
.glyphicon-tags:before {
  content: "\e042";
}
.glyphicon-book:before {
  content: "\e043";
}
.glyphicon-bookmark:before {
  content: "\e044";
}
.glyphicon-print:before {
  content: "\e045";
}
.glyphicon-camera:before {
  content: "\e046";
}
.glyphicon-font:before {
  content: "\e047";
}
.glyphicon-bold:before {
  content: "\e048";
}
.glyphicon-italic:before {
  content: "\e049";
}
.glyphicon-text-height:before {
  content: "\e050";
}
.glyphicon-text-width:before {
  content: "\e051";
}
.glyphicon-align-left:before {
  content: "\e052";
}
.glyphicon-align-center:before {
  content: "\e053";
}
.glyphicon-align-right:before {
  content: "\e054";
}
.glyphicon-align-justify:before {
  content: "\e055";
}
.glyphicon-list:before {
  content: "\e056";
}
.glyphicon-indent-left:before {
  content: "\e057";
}
.glyphicon-indent-right:before {
  content: "\e058";
}
.glyphicon-facetime-video:before {
  content: "\e059";
}
.glyphicon-picture:before {
  content: "\e060";
}
.glyphicon-map-marker:before {
  content: "\e062";
}
.glyphicon-adjust:before {
  content: "\e063";
}
.glyphicon-tint:before {
  content: "\e064";
}
.glyphicon-edit:before {
  content: "\e065";
}
.glyphicon-share:before {
  content: "\e066";
}
.glyphicon-check:before {
  content: "\e067";
}
.glyphicon-move:before {
  content: "\e068";
}
.glyphicon-step-backward:before {
  content: "\e069";
}
.glyphicon-fast-backward:before {
  content: "\e070";
}
.glyphicon-backward:before {
  content: "\e071";
}
.glyphicon-play:before {
  content: "\e072";
}
.glyphicon-pause:before {
  content: "\e073";
}
.glyphicon-stop:before {
  content: "\e074";
}
.glyphicon-forward:before {
  content: "\e075";
}
.glyphicon-fast-forward:before {
  content: "\e076";
}
.glyphicon-step-forward:before {
  content: "\e077";
}
.glyphicon-eject:before {
  content: "\e078";
}
.glyphicon-chevron-left:before {
  content: "\e079";
}
.glyphicon-chevron-right:before {
  content: "\e080";
}
.glyphicon-plus-sign:before {
  content: "\e081";
}
.glyphicon-minus-sign:before {
  content: "\e082";
}
.glyphicon-remove-sign:before {
  content: "\e083";
}
.glyphicon-ok-sign:before {
  content: "\e084";
}
.glyphicon-question-sign:before {
  content: "\e085";
}
.glyphicon-info-sign:before {
  content: "\e086";
}
.glyphicon-screenshot:before {
  content: "\e087";
}
.glyphicon-remove-circle:before {
  content: "\e088";
}
.glyphicon-ok-circle:before {
  content: "\e089";
}
.glyphicon-ban-circle:before {
  content: "\e090";
}
.glyphicon-arrow-left:before {
  content: "\e091";
}
.glyphicon-arrow-right:before {
  content: "\e092";
}
.glyphicon-arrow-up:before {
  content: "\e093";
}
.glyphicon-arrow-down:before {
  content: "\e094";
}
.glyphicon-share-alt:before {
  content: "\e095";
}
.glyphicon-resize-full:before {
  content: "\e096";
}
.glyphicon-resize-small:before {
  content: "\e097";
}
.glyphicon-exclamation-sign:before {
  content: "\e101";
}
.glyphicon-gift:before {
  content: "\e102";
}
.glyphicon-leaf:before {
  content: "\e103";
}
.glyphicon-fire:before {
  content: "\e104";
}
.glyphicon-eye-open:before {
  content: "\e105";
}
.glyphicon-eye-close:before {
  content: "\e106";
}
.glyphicon-warning-sign:before {
  content: "\e107";
}
.glyphicon-plane:before {
  content: "\e108";
}
.glyphicon-calendar:before {
  content: "\e109";
}
.glyphicon-random:before {
  content: "\e110";
}
.glyphicon-comment:before {
  content: "\e111";
}
.glyphicon-magnet:before {
  content: "\e112";
}
.glyphicon-chevron-up:before {
  content: "\e113";
}
.glyphicon-chevron-down:before {
  content: "\e114";
}
.glyphicon-retweet:before {
  content: "\e115";
}
.glyphicon-shopping-cart:before {
  content: "\e116";
}
.glyphicon-folder-close:before {
  content: "\e117";
}
.glyphicon-folder-open:before {
  content: "\e118";
}
.glyphicon-resize-vertical:before {
  content: "\e119";
}
.glyphicon-resize-horizontal:before {
  content: "\e120";
}
.glyphicon-hdd:before {
  content: "\e121";
}
.glyphicon-bullhorn:before {
  content: "\e122";
}
.glyphicon-bell:before {
  content: "\e123";
}
.glyphicon-certificate:before {
  content: "\e124";
}
.glyphicon-thumbs-up:before {
  content: "\e125";
}
.glyphicon-thumbs-down:before {
  content: "\e126";
}
.glyphicon-hand-right:before {
  content: "\e127";
}
.glyphicon-hand-left:before {
  content: "\e128";
}
.glyphicon-hand-up:before {
  content: "\e129";
}
.glyphicon-hand-down:before {
  content: "\e130";
}
.glyphicon-circle-arrow-right:before {
  content: "\e131";
}
.glyphicon-circle-arrow-left:before {
  content: "\e132";
}
.glyphicon-circle-arrow-up:before {
  content: "\e133";
}
.glyphicon-circle-arrow-down:before {
  content: "\e134";
}
.glyphicon-globe:before {
  content: "\e135";
}
.glyphicon-wrench:before {
  content: "\e136";
}
.glyphicon-tasks:before {
  content: "\e137";
}
.glyphicon-filter:before {
  content: "\e138";
}
.glyphicon-briefcase:before {
  content: "\e139";
}
.glyphicon-fullscreen:before {
  content: "\e140";
}
.glyphicon-dashboard:before {
  content: "\e141";
}
.glyphicon-paperclip:before {
  content: "\e142";
}
.glyphicon-heart-empty:before {
  content: "\e143";
}
.glyphicon-link:before {
  content: "\e144";
}
.glyphicon-phone:before {
  content: "\e145";
}
.glyphicon-pushpin:before {
  content: "\e146";
}
.glyphicon-usd:before {
  content: "\e148";
}
.glyphicon-gbp:before {
  content: "\e149";
}
.glyphicon-sort:before {
  content: "\e150";
}
.glyphicon-sort-by-alphabet:before {
  content: "\e151";
}
.glyphicon-sort-by-alphabet-alt:before {
  content: "\e152";
}
.glyphicon-sort-by-order:before {
  content: "\e153";
}
.glyphicon-sort-by-order-alt:before {
  content: "\e154";
}
.glyphicon-sort-by-attributes:before {
  content: "\e155";
}
.glyphicon-sort-by-attributes-alt:before {
  content: "\e156";
}
.glyphicon-unchecked:before {
  content: "\e157";
}
.glyphicon-expand:before {
  content: "\e158";
}
.glyphicon-collapse-down:before {
  content: "\e159";
}
.glyphicon-collapse-up:before {
  content: "\e160";
}
.glyphicon-log-in:before {
  content: "\e161";
}
.glyphicon-flash:before {
  content: "\e162";
}
.glyphicon-log-out:before {
  content: "\e163";
}
.glyphicon-new-window:before {
  content: "\e164";
}
.glyphicon-record:before {
  content: "\e165";
}
.glyphicon-save:before {
  content: "\e166";
}
.glyphicon-open:before {
  content: "\e167";
}
.glyphicon-saved:before {
  content: "\e168";
}
.glyphicon-import:before {
  content: "\e169";
}
.glyphicon-export:before {
  content: "\e170";
}
.glyphicon-send:before {
  content: "\e171";
}
.glyphicon-floppy-disk:before {
  content: "\e172";
}
.glyphicon-floppy-saved:before {
  content: "\e173";
}
.glyphicon-floppy-remove:before {
  content: "\e174";
}
.glyphicon-floppy-save:before {
  content: "\e175";
}
.glyphicon-floppy-open:before {
  content: "\e176";
}
.glyphicon-credit-card:before {
  content: "\e177";
}
.glyphicon-transfer:before {
  content: "\e178";
}
.glyphicon-cutlery:before {
  content: "\e179";
}
.glyphicon-header:before {
  content: "\e180";
}
.glyphicon-compressed:before {
  content: "\e181";
}
.glyphicon-earphone:before {
  content: "\e182";
}
.glyphicon-phone-alt:before {
  content: "\e183";
}
.glyphicon-tower:before {
  content: "\e184";
}
.glyphicon-stats:before {
  content: "\e185";
}
.glyphicon-sd-video:before {
  content: "\e186";
}
.glyphicon-hd-video:before {
  content: "\e187";
}
.glyphicon-subtitles:before {
  content: "\e188";
}
.glyphicon-sound-stereo:before {
  content: "\e189";
}
.glyphicon-sound-dolby:before {
  content: "\e190";
}
.glyphicon-sound-5-1:before {
  content: "\e191";
}
.glyphicon-sound-6-1:before {
  content: "\e192";
}
.glyphicon-sound-7-1:before {
  content: "\e193";
}
.glyphicon-copyright-mark:before {
  content: "\e194";
}
.glyphicon-registration-mark:before {
  content: "\e195";
}
.glyphicon-cloud-download:before {
  content: "\e197";
}
.glyphicon-cloud-upload:before {
  content: "\e198";
}
.glyphicon-tree-conifer:before {
  content: "\e199";
}
.glyphicon-tree-deciduous:before {
  content: "\e200";
}
.glyphicon-cd:before {
  content: "\e201";
}
.glyphicon-save-file:before {
  content: "\e202";
}
.glyphicon-open-file:before {
  content: "\e203";
}
.glyphicon-level-up:before {
  content: "\e204";
}
.glyphicon-copy:before {
  content: "\e205";
}
.glyphicon-paste:before {
  content: "\e206";
}
.glyphicon-alert:before {
  content: "\e209";
}
.glyphicon-equalizer:before {
  content: "\e210";
}
.glyphicon-king:before {
  content: "\e211";
}
.glyphicon-queen:before {
  content: "\e212";
}
.glyphicon-pawn:before {
  content: "\e213";
}
.glyphicon-bishop:before {
  content: "\e214";
}
.glyphicon-knight:before {
  content: "\e215";
}
.glyphicon-baby-formula:before {
  content: "\e216";
}
.glyphicon-tent:before {
  content: "\26fa";
}
.glyphicon-blackboard:before {
  content: "\e218";
}
.glyphicon-bed:before {
  content: "\e219";
}
.glyphicon-apple:before {
  content: "\f8ff";
}
.glyphicon-erase:before {
  content: "\e221";
}
.glyphicon-hourglass:before {
  content: "\231b";
}
.glyphicon-lamp:before {
  content: "\e223";
}
.glyphicon-duplicate:before {
  content: "\e224";
}
.glyphicon-piggy-bank:before {
  content: "\e225";
}
.glyphicon-scissors:before {
  content: "\e226";
}
.glyphicon-bitcoin:before {
  content: "\e227";
}
.glyphicon-btc:before {
  content: "\e227";
}
.glyphicon-xbt:before {
  content: "\e227";
}
.glyphicon-yen:before {
  content: "\00a5";
}
.glyphicon-jpy:before {
  content: "\00a5";
}
.glyphicon-ruble:before {
  content: "\20bd";
}
.glyphicon-rub:before {
  content: "\20bd";
}
.glyphicon-scale:before {
  content: "\e230";
}
.glyphicon-ice-lolly:before {
  content: "\e231";
}
.glyphicon-ice-lolly-tasted:before {
  content: "\e232";
}
.glyphicon-education:before {
  content: "\e233";
}
.glyphicon-option-horizontal:before {
  content: "\e234";
}
.glyphicon-option-vertical:before {
  content: "\e235";
}
.glyphicon-menu-hamburger:before {
  content: "\e236";
}
.glyphicon-modal-window:before {
  content: "\e237";
}
.glyphicon-oil:before {
  content: "\e238";
}
.glyphicon-grain:before {
  content: "\e239";
}
.glyphicon-sunglasses:before {
  content: "\e240";
}
.glyphicon-text-size:before {
  content: "\e241";
}
.glyphicon-text-color:before {
  content: "\e242";
}
.glyphicon-text-background:before {
  content: "\e243";
}
.glyphicon-object-align-top:before {
  content: "\e244";
}
.glyphicon-object-align-bottom:before {
  content: "\e245";
}
.glyphicon-object-align-horizontal:before {
  content: "\e246";
}
.glyphicon-object-align-left:before {
  content: "\e247";
}
.glyphicon-object-align-vertical:before {
  content: "\e248";
}
.glyphicon-object-align-right:before {
  content: "\e249";
}
.glyphicon-triangle-right:before {
  content: "\e250";
}
.glyphicon-triangle-left:before {
  content: "\e251";
}
.glyphicon-triangle-bottom:before {
  content: "\e252";
}
.glyphicon-triangle-top:before {
  content: "\e253";
}
.glyphicon-console:before {
  content: "\e254";
}
.glyphicon-superscript:before {
  content: "\e255";
}
.glyphicon-subscript:before {
  content: "\e256";
}
.glyphicon-menu-left:before {
  content: "\e257";
}
.glyphicon-menu-right:before {
  content: "\e258";
}
.glyphicon-menu-down:before {
  content: "\e259";
}
.glyphicon-menu-up:before {
  content: "\e260";
}
* {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
*:before,
*:after {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
html {
  font-size: 10px;
  -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
}
body {
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-size: 13px;
  line-height: 1.42857143;
  color: #000;
  background-color: #fff;
}
input,
button,
select,
textarea {
  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
}
a {
  color: #337ab7;
  text-decoration: none;
}
a:hover,
a:focus {
  color: #23527c;
  text-decoration: underline;
}
a:focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
figure {
  margin: 0;
}
img {
  vertical-align: middle;
}
.img-responsive,
.thumbnail > img,
.thumbnail a > img,
.carousel-inner > .item > img,
.carousel-inner > .item > a > img {
  display: block;
  max-width: 100%;
  height: auto;
}
.img-rounded {
  border-radius: 3px;
}
.img-thumbnail {
  padding: 4px;
  line-height: 1.42857143;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 2px;
  -webkit-transition: all 0.2s ease-in-out;
  -o-transition: all 0.2s ease-in-out;
  transition: all 0.2s ease-in-out;
  display: inline-block;
  max-width: 100%;
  height: auto;
}
.img-circle {
  border-radius: 50%;
}
hr {
  margin-top: 18px;
  margin-bottom: 18px;
  border: 0;
  border-top: 1px solid #eeeeee;
}
.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  margin: -1px;
  padding: 0;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  border: 0;
}
.sr-only-focusable:active,
.sr-only-focusable:focus {
  position: static;
  width: auto;
  height: auto;
  margin: 0;
  overflow: visible;
  clip: auto;
}
[role="button"] {
  cursor: pointer;
}
h1,
h2,
h3,
h4,
h5,
h6,
.h1,
.h2,
.h3,
.h4,
.h5,
.h6 {
  font-family: inherit;
  font-weight: 500;
  line-height: 1.1;
  color: inherit;
}
h1 small,
h2 small,
h3 small,
h4 small,
h5 small,
h6 small,
.h1 small,
.h2 small,
.h3 small,
.h4 small,
.h5 small,
.h6 small,
h1 .small,
h2 .small,
h3 .small,
h4 .small,
h5 .small,
h6 .small,
.h1 .small,
.h2 .small,
.h3 .small,
.h4 .small,
.h5 .small,
.h6 .small {
  font-weight: normal;
  line-height: 1;
  color: #777777;
}
h1,
.h1,
h2,
.h2,
h3,
.h3 {
  margin-top: 18px;
  margin-bottom: 9px;
}
h1 small,
.h1 small,
h2 small,
.h2 small,
h3 small,
.h3 small,
h1 .small,
.h1 .small,
h2 .small,
.h2 .small,
h3 .small,
.h3 .small {
  font-size: 65%;
}
h4,
.h4,
h5,
.h5,
h6,
.h6 {
  margin-top: 9px;
  margin-bottom: 9px;
}
h4 small,
.h4 small,
h5 small,
.h5 small,
h6 small,
.h6 small,
h4 .small,
.h4 .small,
h5 .small,
.h5 .small,
h6 .small,
.h6 .small {
  font-size: 75%;
}
h1,
.h1 {
  font-size: 33px;
}
h2,
.h2 {
  font-size: 27px;
}
h3,
.h3 {
  font-size: 23px;
}
h4,
.h4 {
  font-size: 17px;
}
h5,
.h5 {
  font-size: 13px;
}
h6,
.h6 {
  font-size: 12px;
}
p {
  margin: 0 0 9px;
}
.lead {
  margin-bottom: 18px;
  font-size: 14px;
  font-weight: 300;
  line-height: 1.4;
}
@media (min-width: 768px) {
  .lead {
    font-size: 19.5px;
  }
}
small,
.small {
  font-size: 92%;
}
mark,
.mark {
  background-color: #fcf8e3;
  padding: .2em;
}
.text-left {
  text-align: left;
}
.text-right {
  text-align: right;
}
.text-center {
  text-align: center;
}
.text-justify {
  text-align: justify;
}
.text-nowrap {
  white-space: nowrap;
}
.text-lowercase {
  text-transform: lowercase;
}
.text-uppercase {
  text-transform: uppercase;
}
.text-capitalize {
  text-transform: capitalize;
}
.text-muted {
  color: #777777;
}
.text-primary {
  color: #337ab7;
}
a.text-primary:hover,
a.text-primary:focus {
  color: #286090;
}
.text-success {
  color: #3c763d;
}
a.text-success:hover,
a.text-success:focus {
  color: #2b542c;
}
.text-info {
  color: #31708f;
}
a.text-info:hover,
a.text-info:focus {
  color: #245269;
}
.text-warning {
  color: #8a6d3b;
}
a.text-warning:hover,
a.text-warning:focus {
  color: #66512c;
}
.text-danger {
  color: #a94442;
}
a.text-danger:hover,
a.text-danger:focus {
  color: #843534;
}
.bg-primary {
  color: #fff;
  background-color: #337ab7;
}
a.bg-primary:hover,
a.bg-primary:focus {
  background-color: #286090;
}
.bg-success {
  background-color: #dff0d8;
}
a.bg-success:hover,
a.bg-success:focus {
  background-color: #c1e2b3;
}
.bg-info {
  background-color: #d9edf7;
}
a.bg-info:hover,
a.bg-info:focus {
  background-color: #afd9ee;
}
.bg-warning {
  background-color: #fcf8e3;
}
a.bg-warning:hover,
a.bg-warning:focus {
  background-color: #f7ecb5;
}
.bg-danger {
  background-color: #f2dede;
}
a.bg-danger:hover,
a.bg-danger:focus {
  background-color: #e4b9b9;
}
.page-header {
  padding-bottom: 8px;
  margin: 36px 0 18px;
  border-bottom: 1px solid #eeeeee;
}
ul,
ol {
  margin-top: 0;
  margin-bottom: 9px;
}
ul ul,
ol ul,
ul ol,
ol ol {
  margin-bottom: 0;
}
.list-unstyled {
  padding-left: 0;
  list-style: none;
}
.list-inline {
  padding-left: 0;
  list-style: none;
  margin-left: -5px;
}
.list-inline > li {
  display: inline-block;
  padding-left: 5px;
  padding-right: 5px;
}
dl {
  margin-top: 0;
  margin-bottom: 18px;
}
dt,
dd {
  line-height: 1.42857143;
}
dt {
  font-weight: bold;
}
dd {
  margin-left: 0;
}
@media (min-width: 541px) {
  .dl-horizontal dt {
    float: left;
    width: 160px;
    clear: left;
    text-align: right;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
  }
  .dl-horizontal dd {
    margin-left: 180px;
  }
}
abbr[title],
abbr[data-original-title] {
  cursor: help;
  border-bottom: 1px dotted #777777;
}
.initialism {
  font-size: 90%;
  text-transform: uppercase;
}
blockquote {
  padding: 9px 18px;
  margin: 0 0 18px;
  font-size: inherit;
  border-left: 5px solid #eeeeee;
}
blockquote p:last-child,
blockquote ul:last-child,
blockquote ol:last-child {
  margin-bottom: 0;
}
blockquote footer,
blockquote small,
blockquote .small {
  display: block;
  font-size: 80%;
  line-height: 1.42857143;
  color: #777777;
}
blockquote footer:before,
blockquote small:before,
blockquote .small:before {
  content: '\2014 \00A0';
}
.blockquote-reverse,
blockquote.pull-right {
  padding-right: 15px;
  padding-left: 0;
  border-right: 5px solid #eeeeee;
  border-left: 0;
  text-align: right;
}
.blockquote-reverse footer:before,
blockquote.pull-right footer:before,
.blockquote-reverse small:before,
blockquote.pull-right small:before,
.blockquote-reverse .small:before,
blockquote.pull-right .small:before {
  content: '';
}
.blockquote-reverse footer:after,
blockquote.pull-right footer:after,
.blockquote-reverse small:after,
blockquote.pull-right small:after,
.blockquote-reverse .small:after,
blockquote.pull-right .small:after {
  content: '\00A0 \2014';
}
address {
  margin-bottom: 18px;
  font-style: normal;
  line-height: 1.42857143;
}
code,
kbd,
pre,
samp {
  font-family: monospace;
}
code {
  padding: 2px 4px;
  font-size: 90%;
  color: #c7254e;
  background-color: #f9f2f4;
  border-radius: 2px;
}
kbd {
  padding: 2px 4px;
  font-size: 90%;
  color: #888;
  background-color: transparent;
  border-radius: 1px;
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.25);
}
kbd kbd {
  padding: 0;
  font-size: 100%;
  font-weight: bold;
  box-shadow: none;
}
pre {
  display: block;
  padding: 8.5px;
  margin: 0 0 9px;
  font-size: 12px;
  line-height: 1.42857143;
  word-break: break-all;
  word-wrap: break-word;
  color: #333333;
  background-color: #f5f5f5;
  border: 1px solid #ccc;
  border-radius: 2px;
}
pre code {
  padding: 0;
  font-size: inherit;
  color: inherit;
  white-space: pre-wrap;
  background-color: transparent;
  border-radius: 0;
}
.pre-scrollable {
  max-height: 340px;
  overflow-y: scroll;
}
.container {
  margin-right: auto;
  margin-left: auto;
  padding-left: 0px;
  padding-right: 0px;
}
@media (min-width: 768px) {
  .container {
    width: 768px;
  }
}
@media (min-width: 992px) {
  .container {
    width: 940px;
  }
}
@media (min-width: 1200px) {
  .container {
    width: 1140px;
  }
}
.container-fluid {
  margin-right: auto;
  margin-left: auto;
  padding-left: 0px;
  padding-right: 0px;
}
.row {
  margin-left: 0px;
  margin-right: 0px;
}
.col-xs-1, .col-sm-1, .col-md-1, .col-lg-1, .col-xs-2, .col-sm-2, .col-md-2, .col-lg-2, .col-xs-3, .col-sm-3, .col-md-3, .col-lg-3, .col-xs-4, .col-sm-4, .col-md-4, .col-lg-4, .col-xs-5, .col-sm-5, .col-md-5, .col-lg-5, .col-xs-6, .col-sm-6, .col-md-6, .col-lg-6, .col-xs-7, .col-sm-7, .col-md-7, .col-lg-7, .col-xs-8, .col-sm-8, .col-md-8, .col-lg-8, .col-xs-9, .col-sm-9, .col-md-9, .col-lg-9, .col-xs-10, .col-sm-10, .col-md-10, .col-lg-10, .col-xs-11, .col-sm-11, .col-md-11, .col-lg-11, .col-xs-12, .col-sm-12, .col-md-12, .col-lg-12 {
  position: relative;
  min-height: 1px;
  padding-left: 0px;
  padding-right: 0px;
}
.col-xs-1, .col-xs-2, .col-xs-3, .col-xs-4, .col-xs-5, .col-xs-6, .col-xs-7, .col-xs-8, .col-xs-9, .col-xs-10, .col-xs-11, .col-xs-12 {
  float: left;
}
.col-xs-12 {
  width: 100%;
}
.col-xs-11 {
  width: 91.66666667%;
}
.col-xs-10 {
  width: 83.33333333%;
}
.col-xs-9 {
  width: 75%;
}
.col-xs-8 {
  width: 66.66666667%;
}
.col-xs-7 {
  width: 58.33333333%;
}
.col-xs-6 {
  width: 50%;
}
.col-xs-5 {
  width: 41.66666667%;
}
.col-xs-4 {
  width: 33.33333333%;
}
.col-xs-3 {
  width: 25%;
}
.col-xs-2 {
  width: 16.66666667%;
}
.col-xs-1 {
  width: 8.33333333%;
}
.col-xs-pull-12 {
  right: 100%;
}
.col-xs-pull-11 {
  right: 91.66666667%;
}
.col-xs-pull-10 {
  right: 83.33333333%;
}
.col-xs-pull-9 {
  right: 75%;
}
.col-xs-pull-8 {
  right: 66.66666667%;
}
.col-xs-pull-7 {
  right: 58.33333333%;
}
.col-xs-pull-6 {
  right: 50%;
}
.col-xs-pull-5 {
  right: 41.66666667%;
}
.col-xs-pull-4 {
  right: 33.33333333%;
}
.col-xs-pull-3 {
  right: 25%;
}
.col-xs-pull-2 {
  right: 16.66666667%;
}
.col-xs-pull-1 {
  right: 8.33333333%;
}
.col-xs-pull-0 {
  right: auto;
}
.col-xs-push-12 {
  left: 100%;
}
.col-xs-push-11 {
  left: 91.66666667%;
}
.col-xs-push-10 {
  left: 83.33333333%;
}
.col-xs-push-9 {
  left: 75%;
}
.col-xs-push-8 {
  left: 66.66666667%;
}
.col-xs-push-7 {
  left: 58.33333333%;
}
.col-xs-push-6 {
  left: 50%;
}
.col-xs-push-5 {
  left: 41.66666667%;
}
.col-xs-push-4 {
  left: 33.33333333%;
}
.col-xs-push-3 {
  left: 25%;
}
.col-xs-push-2 {
  left: 16.66666667%;
}
.col-xs-push-1 {
  left: 8.33333333%;
}
.col-xs-push-0 {
  left: auto;
}
.col-xs-offset-12 {
  margin-left: 100%;
}
.col-xs-offset-11 {
  margin-left: 91.66666667%;
}
.col-xs-offset-10 {
  margin-left: 83.33333333%;
}
.col-xs-offset-9 {
  margin-left: 75%;
}
.col-xs-offset-8 {
  margin-left: 66.66666667%;
}
.col-xs-offset-7 {
  margin-left: 58.33333333%;
}
.col-xs-offset-6 {
  margin-left: 50%;
}
.col-xs-offset-5 {
  margin-left: 41.66666667%;
}
.col-xs-offset-4 {
  margin-left: 33.33333333%;
}
.col-xs-offset-3 {
  margin-left: 25%;
}
.col-xs-offset-2 {
  margin-left: 16.66666667%;
}
.col-xs-offset-1 {
  margin-left: 8.33333333%;
}
.col-xs-offset-0 {
  margin-left: 0%;
}
@media (min-width: 768px) {
  .col-sm-1, .col-sm-2, .col-sm-3, .col-sm-4, .col-sm-5, .col-sm-6, .col-sm-7, .col-sm-8, .col-sm-9, .col-sm-10, .col-sm-11, .col-sm-12 {
    float: left;
  }
  .col-sm-12 {
    width: 100%;
  }
  .col-sm-11 {
    width: 91.66666667%;
  }
  .col-sm-10 {
    width: 83.33333333%;
  }
  .col-sm-9 {
    width: 75%;
  }
  .col-sm-8 {
    width: 66.66666667%;
  }
  .col-sm-7 {
    width: 58.33333333%;
  }
  .col-sm-6 {
    width: 50%;
  }
  .col-sm-5 {
    width: 41.66666667%;
  }
  .col-sm-4 {
    width: 33.33333333%;
  }
  .col-sm-3 {
    width: 25%;
  }
  .col-sm-2 {
    width: 16.66666667%;
  }
  .col-sm-1 {
    width: 8.33333333%;
  }
  .col-sm-pull-12 {
    right: 100%;
  }
  .col-sm-pull-11 {
    right: 91.66666667%;
  }
  .col-sm-pull-10 {
    right: 83.33333333%;
  }
  .col-sm-pull-9 {
    right: 75%;
  }
  .col-sm-pull-8 {
    right: 66.66666667%;
  }
  .col-sm-pull-7 {
    right: 58.33333333%;
  }
  .col-sm-pull-6 {
    right: 50%;
  }
  .col-sm-pull-5 {
    right: 41.66666667%;
  }
  .col-sm-pull-4 {
    right: 33.33333333%;
  }
  .col-sm-pull-3 {
    right: 25%;
  }
  .col-sm-pull-2 {
    right: 16.66666667%;
  }
  .col-sm-pull-1 {
    right: 8.33333333%;
  }
  .col-sm-pull-0 {
    right: auto;
  }
  .col-sm-push-12 {
    left: 100%;
  }
  .col-sm-push-11 {
    left: 91.66666667%;
  }
  .col-sm-push-10 {
    left: 83.33333333%;
  }
  .col-sm-push-9 {
    left: 75%;
  }
  .col-sm-push-8 {
    left: 66.66666667%;
  }
  .col-sm-push-7 {
    left: 58.33333333%;
  }
  .col-sm-push-6 {
    left: 50%;
  }
  .col-sm-push-5 {
    left: 41.66666667%;
  }
  .col-sm-push-4 {
    left: 33.33333333%;
  }
  .col-sm-push-3 {
    left: 25%;
  }
  .col-sm-push-2 {
    left: 16.66666667%;
  }
  .col-sm-push-1 {
    left: 8.33333333%;
  }
  .col-sm-push-0 {
    left: auto;
  }
  .col-sm-offset-12 {
    margin-left: 100%;
  }
  .col-sm-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-sm-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-sm-offset-9 {
    margin-left: 75%;
  }
  .col-sm-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-sm-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-sm-offset-6 {
    margin-left: 50%;
  }
  .col-sm-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-sm-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-sm-offset-3 {
    margin-left: 25%;
  }
  .col-sm-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-sm-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-sm-offset-0 {
    margin-left: 0%;
  }
}
@media (min-width: 992px) {
  .col-md-1, .col-md-2, .col-md-3, .col-md-4, .col-md-5, .col-md-6, .col-md-7, .col-md-8, .col-md-9, .col-md-10, .col-md-11, .col-md-12 {
    float: left;
  }
  .col-md-12 {
    width: 100%;
  }
  .col-md-11 {
    width: 91.66666667%;
  }
  .col-md-10 {
    width: 83.33333333%;
  }
  .col-md-9 {
    width: 75%;
  }
  .col-md-8 {
    width: 66.66666667%;
  }
  .col-md-7 {
    width: 58.33333333%;
  }
  .col-md-6 {
    width: 50%;
  }
  .col-md-5 {
    width: 41.66666667%;
  }
  .col-md-4 {
    width: 33.33333333%;
  }
  .col-md-3 {
    width: 25%;
  }
  .col-md-2 {
    width: 16.66666667%;
  }
  .col-md-1 {
    width: 8.33333333%;
  }
  .col-md-pull-12 {
    right: 100%;
  }
  .col-md-pull-11 {
    right: 91.66666667%;
  }
  .col-md-pull-10 {
    right: 83.33333333%;
  }
  .col-md-pull-9 {
    right: 75%;
  }
  .col-md-pull-8 {
    right: 66.66666667%;
  }
  .col-md-pull-7 {
    right: 58.33333333%;
  }
  .col-md-pull-6 {
    right: 50%;
  }
  .col-md-pull-5 {
    right: 41.66666667%;
  }
  .col-md-pull-4 {
    right: 33.33333333%;
  }
  .col-md-pull-3 {
    right: 25%;
  }
  .col-md-pull-2 {
    right: 16.66666667%;
  }
  .col-md-pull-1 {
    right: 8.33333333%;
  }
  .col-md-pull-0 {
    right: auto;
  }
  .col-md-push-12 {
    left: 100%;
  }
  .col-md-push-11 {
    left: 91.66666667%;
  }
  .col-md-push-10 {
    left: 83.33333333%;
  }
  .col-md-push-9 {
    left: 75%;
  }
  .col-md-push-8 {
    left: 66.66666667%;
  }
  .col-md-push-7 {
    left: 58.33333333%;
  }
  .col-md-push-6 {
    left: 50%;
  }
  .col-md-push-5 {
    left: 41.66666667%;
  }
  .col-md-push-4 {
    left: 33.33333333%;
  }
  .col-md-push-3 {
    left: 25%;
  }
  .col-md-push-2 {
    left: 16.66666667%;
  }
  .col-md-push-1 {
    left: 8.33333333%;
  }
  .col-md-push-0 {
    left: auto;
  }
  .col-md-offset-12 {
    margin-left: 100%;
  }
  .col-md-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-md-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-md-offset-9 {
    margin-left: 75%;
  }
  .col-md-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-md-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-md-offset-6 {
    margin-left: 50%;
  }
  .col-md-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-md-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-md-offset-3 {
    margin-left: 25%;
  }
  .col-md-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-md-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-md-offset-0 {
    margin-left: 0%;
  }
}
@media (min-width: 1200px) {
  .col-lg-1, .col-lg-2, .col-lg-3, .col-lg-4, .col-lg-5, .col-lg-6, .col-lg-7, .col-lg-8, .col-lg-9, .col-lg-10, .col-lg-11, .col-lg-12 {
    float: left;
  }
  .col-lg-12 {
    width: 100%;
  }
  .col-lg-11 {
    width: 91.66666667%;
  }
  .col-lg-10 {
    width: 83.33333333%;
  }
  .col-lg-9 {
    width: 75%;
  }
  .col-lg-8 {
    width: 66.66666667%;
  }
  .col-lg-7 {
    width: 58.33333333%;
  }
  .col-lg-6 {
    width: 50%;
  }
  .col-lg-5 {
    width: 41.66666667%;
  }
  .col-lg-4 {
    width: 33.33333333%;
  }
  .col-lg-3 {
    width: 25%;
  }
  .col-lg-2 {
    width: 16.66666667%;
  }
  .col-lg-1 {
    width: 8.33333333%;
  }
  .col-lg-pull-12 {
    right: 100%;
  }
  .col-lg-pull-11 {
    right: 91.66666667%;
  }
  .col-lg-pull-10 {
    right: 83.33333333%;
  }
  .col-lg-pull-9 {
    right: 75%;
  }
  .col-lg-pull-8 {
    right: 66.66666667%;
  }
  .col-lg-pull-7 {
    right: 58.33333333%;
  }
  .col-lg-pull-6 {
    right: 50%;
  }
  .col-lg-pull-5 {
    right: 41.66666667%;
  }
  .col-lg-pull-4 {
    right: 33.33333333%;
  }
  .col-lg-pull-3 {
    right: 25%;
  }
  .col-lg-pull-2 {
    right: 16.66666667%;
  }
  .col-lg-pull-1 {
    right: 8.33333333%;
  }
  .col-lg-pull-0 {
    right: auto;
  }
  .col-lg-push-12 {
    left: 100%;
  }
  .col-lg-push-11 {
    left: 91.66666667%;
  }
  .col-lg-push-10 {
    left: 83.33333333%;
  }
  .col-lg-push-9 {
    left: 75%;
  }
  .col-lg-push-8 {
    left: 66.66666667%;
  }
  .col-lg-push-7 {
    left: 58.33333333%;
  }
  .col-lg-push-6 {
    left: 50%;
  }
  .col-lg-push-5 {
    left: 41.66666667%;
  }
  .col-lg-push-4 {
    left: 33.33333333%;
  }
  .col-lg-push-3 {
    left: 25%;
  }
  .col-lg-push-2 {
    left: 16.66666667%;
  }
  .col-lg-push-1 {
    left: 8.33333333%;
  }
  .col-lg-push-0 {
    left: auto;
  }
  .col-lg-offset-12 {
    margin-left: 100%;
  }
  .col-lg-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-lg-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-lg-offset-9 {
    margin-left: 75%;
  }
  .col-lg-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-lg-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-lg-offset-6 {
    margin-left: 50%;
  }
  .col-lg-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-lg-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-lg-offset-3 {
    margin-left: 25%;
  }
  .col-lg-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-lg-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-lg-offset-0 {
    margin-left: 0%;
  }
}
table {
  background-color: transparent;
}
caption {
  padding-top: 8px;
  padding-bottom: 8px;
  color: #777777;
  text-align: left;
}
th {
  text-align: left;
}
.table {
  width: 100%;
  max-width: 100%;
  margin-bottom: 18px;
}
.table > thead > tr > th,
.table > tbody > tr > th,
.table > tfoot > tr > th,
.table > thead > tr > td,
.table > tbody > tr > td,
.table > tfoot > tr > td {
  padding: 8px;
  line-height: 1.42857143;
  vertical-align: top;
  border-top: 1px solid #ddd;
}
.table > thead > tr > th {
  vertical-align: bottom;
  border-bottom: 2px solid #ddd;
}
.table > caption + thead > tr:first-child > th,
.table > colgroup + thead > tr:first-child > th,
.table > thead:first-child > tr:first-child > th,
.table > caption + thead > tr:first-child > td,
.table > colgroup + thead > tr:first-child > td,
.table > thead:first-child > tr:first-child > td {
  border-top: 0;
}
.table > tbody + tbody {
  border-top: 2px solid #ddd;
}
.table .table {
  background-color: #fff;
}
.table-condensed > thead > tr > th,
.table-condensed > tbody > tr > th,
.table-condensed > tfoot > tr > th,
.table-condensed > thead > tr > td,
.table-condensed > tbody > tr > td,
.table-condensed > tfoot > tr > td {
  padding: 5px;
}
.table-bordered {
  border: 1px solid #ddd;
}
.table-bordered > thead > tr > th,
.table-bordered > tbody > tr > th,
.table-bordered > tfoot > tr > th,
.table-bordered > thead > tr > td,
.table-bordered > tbody > tr > td,
.table-bordered > tfoot > tr > td {
  border: 1px solid #ddd;
}
.table-bordered > thead > tr > th,
.table-bordered > thead > tr > td {
  border-bottom-width: 2px;
}
.table-striped > tbody > tr:nth-of-type(odd) {
  background-color: #f9f9f9;
}
.table-hover > tbody > tr:hover {
  background-color: #f5f5f5;
}
table col[class*="col-"] {
  position: static;
  float: none;
  display: table-column;
}
table td[class*="col-"],
table th[class*="col-"] {
  position: static;
  float: none;
  display: table-cell;
}
.table > thead > tr > td.active,
.table > tbody > tr > td.active,
.table > tfoot > tr > td.active,
.table > thead > tr > th.active,
.table > tbody > tr > th.active,
.table > tfoot > tr > th.active,
.table > thead > tr.active > td,
.table > tbody > tr.active > td,
.table > tfoot > tr.active > td,
.table > thead > tr.active > th,
.table > tbody > tr.active > th,
.table > tfoot > tr.active > th {
  background-color: #f5f5f5;
}
.table-hover > tbody > tr > td.active:hover,
.table-hover > tbody > tr > th.active:hover,
.table-hover > tbody > tr.active:hover > td,
.table-hover > tbody > tr:hover > .active,
.table-hover > tbody > tr.active:hover > th {
  background-color: #e8e8e8;
}
.table > thead > tr > td.success,
.table > tbody > tr > td.success,
.table > tfoot > tr > td.success,
.table > thead > tr > th.success,
.table > tbody > tr > th.success,
.table > tfoot > tr > th.success,
.table > thead > tr.success > td,
.table > tbody > tr.success > td,
.table > tfoot > tr.success > td,
.table > thead > tr.success > th,
.table > tbody > tr.success > th,
.table > tfoot > tr.success > th {
  background-color: #dff0d8;
}
.table-hover > tbody > tr > td.success:hover,
.table-hover > tbody > tr > th.success:hover,
.table-hover > tbody > tr.success:hover > td,
.table-hover > tbody > tr:hover > .success,
.table-hover > tbody > tr.success:hover > th {
  background-color: #d0e9c6;
}
.table > thead > tr > td.info,
.table > tbody > tr > td.info,
.table > tfoot > tr > td.info,
.table > thead > tr > th.info,
.table > tbody > tr > th.info,
.table > tfoot > tr > th.info,
.table > thead > tr.info > td,
.table > tbody > tr.info > td,
.table > tfoot > tr.info > td,
.table > thead > tr.info > th,
.table > tbody > tr.info > th,
.table > tfoot > tr.info > th {
  background-color: #d9edf7;
}
.table-hover > tbody > tr > td.info:hover,
.table-hover > tbody > tr > th.info:hover,
.table-hover > tbody > tr.info:hover > td,
.table-hover > tbody > tr:hover > .info,
.table-hover > tbody > tr.info:hover > th {
  background-color: #c4e3f3;
}
.table > thead > tr > td.warning,
.table > tbody > tr > td.warning,
.table > tfoot > tr > td.warning,
.table > thead > tr > th.warning,
.table > tbody > tr > th.warning,
.table > tfoot > tr > th.warning,
.table > thead > tr.warning > td,
.table > tbody > tr.warning > td,
.table > tfoot > tr.warning > td,
.table > thead > tr.warning > th,
.table > tbody > tr.warning > th,
.table > tfoot > tr.warning > th {
  background-color: #fcf8e3;
}
.table-hover > tbody > tr > td.warning:hover,
.table-hover > tbody > tr > th.warning:hover,
.table-hover > tbody > tr.warning:hover > td,
.table-hover > tbody > tr:hover > .warning,
.table-hover > tbody > tr.warning:hover > th {
  background-color: #faf2cc;
}
.table > thead > tr > td.danger,
.table > tbody > tr > td.danger,
.table > tfoot > tr > td.danger,
.table > thead > tr > th.danger,
.table > tbody > tr > th.danger,
.table > tfoot > tr > th.danger,
.table > thead > tr.danger > td,
.table > tbody > tr.danger > td,
.table > tfoot > tr.danger > td,
.table > thead > tr.danger > th,
.table > tbody > tr.danger > th,
.table > tfoot > tr.danger > th {
  background-color: #f2dede;
}
.table-hover > tbody > tr > td.danger:hover,
.table-hover > tbody > tr > th.danger:hover,
.table-hover > tbody > tr.danger:hover > td,
.table-hover > tbody > tr:hover > .danger,
.table-hover > tbody > tr.danger:hover > th {
  background-color: #ebcccc;
}
.table-responsive {
  overflow-x: auto;
  min-height: 0.01%;
}
@media screen and (max-width: 767px) {
  .table-responsive {
    width: 100%;
    margin-bottom: 13.5px;
    overflow-y: hidden;
    -ms-overflow-style: -ms-autohiding-scrollbar;
    border: 1px solid #ddd;
  }
  .table-responsive > .table {
    margin-bottom: 0;
  }
  .table-responsive > .table > thead > tr > th,
  .table-responsive > .table > tbody > tr > th,
  .table-responsive > .table > tfoot > tr > th,
  .table-responsive > .table > thead > tr > td,
  .table-responsive > .table > tbody > tr > td,
  .table-responsive > .table > tfoot > tr > td {
    white-space: nowrap;
  }
  .table-responsive > .table-bordered {
    border: 0;
  }
  .table-responsive > .table-bordered > thead > tr > th:first-child,
  .table-responsive > .table-bordered > tbody > tr > th:first-child,
  .table-responsive > .table-bordered > tfoot > tr > th:first-child,
  .table-responsive > .table-bordered > thead > tr > td:first-child,
  .table-responsive > .table-bordered > tbody > tr > td:first-child,
  .table-responsive > .table-bordered > tfoot > tr > td:first-child {
    border-left: 0;
  }
  .table-responsive > .table-bordered > thead > tr > th:last-child,
  .table-responsive > .table-bordered > tbody > tr > th:last-child,
  .table-responsive > .table-bordered > tfoot > tr > th:last-child,
  .table-responsive > .table-bordered > thead > tr > td:last-child,
  .table-responsive > .table-bordered > tbody > tr > td:last-child,
  .table-responsive > .table-bordered > tfoot > tr > td:last-child {
    border-right: 0;
  }
  .table-responsive > .table-bordered > tbody > tr:last-child > th,
  .table-responsive > .table-bordered > tfoot > tr:last-child > th,
  .table-responsive > .table-bordered > tbody > tr:last-child > td,
  .table-responsive > .table-bordered > tfoot > tr:last-child > td {
    border-bottom: 0;
  }
}
fieldset {
  padding: 0;
  margin: 0;
  border: 0;
  min-width: 0;
}
legend {
  display: block;
  width: 100%;
  padding: 0;
  margin-bottom: 18px;
  font-size: 19.5px;
  line-height: inherit;
  color: #333333;
  border: 0;
  border-bottom: 1px solid #e5e5e5;
}
label {
  display: inline-block;
  max-width: 100%;
  margin-bottom: 5px;
  font-weight: bold;
}
input[type="search"] {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
input[type="radio"],
input[type="checkbox"] {
  margin: 4px 0 0;
  margin-top: 1px \9;
  line-height: normal;
}
input[type="file"] {
  display: block;
}
input[type="range"] {
  display: block;
  width: 100%;
}
select[multiple],
select[size] {
  height: auto;
}
input[type="file"]:focus,
input[type="radio"]:focus,
input[type="checkbox"]:focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
output {
  display: block;
  padding-top: 7px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
}
.form-control {
  display: block;
  width: 100%;
  height: 32px;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
}
.form-control:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.form-control::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.form-control:-ms-input-placeholder {
  color: #999;
}
.form-control::-webkit-input-placeholder {
  color: #999;
}
.form-control::-ms-expand {
  border: 0;
  background-color: transparent;
}
.form-control[disabled],
.form-control[readonly],
fieldset[disabled] .form-control {
  background-color: #eeeeee;
  opacity: 1;
}
.form-control[disabled],
fieldset[disabled] .form-control {
  cursor: not-allowed;
}
textarea.form-control {
  height: auto;
}
input[type="search"] {
  -webkit-appearance: none;
}
@media screen and (-webkit-min-device-pixel-ratio: 0) {
  input[type="date"].form-control,
  input[type="time"].form-control,
  input[type="datetime-local"].form-control,
  input[type="month"].form-control {
    line-height: 32px;
  }
  input[type="date"].input-sm,
  input[type="time"].input-sm,
  input[type="datetime-local"].input-sm,
  input[type="month"].input-sm,
  .input-group-sm input[type="date"],
  .input-group-sm input[type="time"],
  .input-group-sm input[type="datetime-local"],
  .input-group-sm input[type="month"] {
    line-height: 30px;
  }
  input[type="date"].input-lg,
  input[type="time"].input-lg,
  input[type="datetime-local"].input-lg,
  input[type="month"].input-lg,
  .input-group-lg input[type="date"],
  .input-group-lg input[type="time"],
  .input-group-lg input[type="datetime-local"],
  .input-group-lg input[type="month"] {
    line-height: 45px;
  }
}
.form-group {
  margin-bottom: 15px;
}
.radio,
.checkbox {
  position: relative;
  display: block;
  margin-top: 10px;
  margin-bottom: 10px;
}
.radio label,
.checkbox label {
  min-height: 18px;
  padding-left: 20px;
  margin-bottom: 0;
  font-weight: normal;
  cursor: pointer;
}
.radio input[type="radio"],
.radio-inline input[type="radio"],
.checkbox input[type="checkbox"],
.checkbox-inline input[type="checkbox"] {
  position: absolute;
  margin-left: -20px;
  margin-top: 4px \9;
}
.radio + .radio,
.checkbox + .checkbox {
  margin-top: -5px;
}
.radio-inline,
.checkbox-inline {
  position: relative;
  display: inline-block;
  padding-left: 20px;
  margin-bottom: 0;
  vertical-align: middle;
  font-weight: normal;
  cursor: pointer;
}
.radio-inline + .radio-inline,
.checkbox-inline + .checkbox-inline {
  margin-top: 0;
  margin-left: 10px;
}
input[type="radio"][disabled],
input[type="checkbox"][disabled],
input[type="radio"].disabled,
input[type="checkbox"].disabled,
fieldset[disabled] input[type="radio"],
fieldset[disabled] input[type="checkbox"] {
  cursor: not-allowed;
}
.radio-inline.disabled,
.checkbox-inline.disabled,
fieldset[disabled] .radio-inline,
fieldset[disabled] .checkbox-inline {
  cursor: not-allowed;
}
.radio.disabled label,
.checkbox.disabled label,
fieldset[disabled] .radio label,
fieldset[disabled] .checkbox label {
  cursor: not-allowed;
}
.form-control-static {
  padding-top: 7px;
  padding-bottom: 7px;
  margin-bottom: 0;
  min-height: 31px;
}
.form-control-static.input-lg,
.form-control-static.input-sm {
  padding-left: 0;
  padding-right: 0;
}
.input-sm {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
select.input-sm {
  height: 30px;
  line-height: 30px;
}
textarea.input-sm,
select[multiple].input-sm {
  height: auto;
}
.form-group-sm .form-control {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.form-group-sm select.form-control {
  height: 30px;
  line-height: 30px;
}
.form-group-sm textarea.form-control,
.form-group-sm select[multiple].form-control {
  height: auto;
}
.form-group-sm .form-control-static {
  height: 30px;
  min-height: 30px;
  padding: 6px 10px;
  font-size: 12px;
  line-height: 1.5;
}
.input-lg {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
select.input-lg {
  height: 45px;
  line-height: 45px;
}
textarea.input-lg,
select[multiple].input-lg {
  height: auto;
}
.form-group-lg .form-control {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
.form-group-lg select.form-control {
  height: 45px;
  line-height: 45px;
}
.form-group-lg textarea.form-control,
.form-group-lg select[multiple].form-control {
  height: auto;
}
.form-group-lg .form-control-static {
  height: 45px;
  min-height: 35px;
  padding: 11px 16px;
  font-size: 17px;
  line-height: 1.3333333;
}
.has-feedback {
  position: relative;
}
.has-feedback .form-control {
  padding-right: 40px;
}
.form-control-feedback {
  position: absolute;
  top: 0;
  right: 0;
  z-index: 2;
  display: block;
  width: 32px;
  height: 32px;
  line-height: 32px;
  text-align: center;
  pointer-events: none;
}
.input-lg + .form-control-feedback,
.input-group-lg + .form-control-feedback,
.form-group-lg .form-control + .form-control-feedback {
  width: 45px;
  height: 45px;
  line-height: 45px;
}
.input-sm + .form-control-feedback,
.input-group-sm + .form-control-feedback,
.form-group-sm .form-control + .form-control-feedback {
  width: 30px;
  height: 30px;
  line-height: 30px;
}
.has-success .help-block,
.has-success .control-label,
.has-success .radio,
.has-success .checkbox,
.has-success .radio-inline,
.has-success .checkbox-inline,
.has-success.radio label,
.has-success.checkbox label,
.has-success.radio-inline label,
.has-success.checkbox-inline label {
  color: #3c763d;
}
.has-success .form-control {
  border-color: #3c763d;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-success .form-control:focus {
  border-color: #2b542c;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #67b168;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #67b168;
}
.has-success .input-group-addon {
  color: #3c763d;
  border-color: #3c763d;
  background-color: #dff0d8;
}
.has-success .form-control-feedback {
  color: #3c763d;
}
.has-warning .help-block,
.has-warning .control-label,
.has-warning .radio,
.has-warning .checkbox,
.has-warning .radio-inline,
.has-warning .checkbox-inline,
.has-warning.radio label,
.has-warning.checkbox label,
.has-warning.radio-inline label,
.has-warning.checkbox-inline label {
  color: #8a6d3b;
}
.has-warning .form-control {
  border-color: #8a6d3b;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-warning .form-control:focus {
  border-color: #66512c;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #c0a16b;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #c0a16b;
}
.has-warning .input-group-addon {
  color: #8a6d3b;
  border-color: #8a6d3b;
  background-color: #fcf8e3;
}
.has-warning .form-control-feedback {
  color: #8a6d3b;
}
.has-error .help-block,
.has-error .control-label,
.has-error .radio,
.has-error .checkbox,
.has-error .radio-inline,
.has-error .checkbox-inline,
.has-error.radio label,
.has-error.checkbox label,
.has-error.radio-inline label,
.has-error.checkbox-inline label {
  color: #a94442;
}
.has-error .form-control {
  border-color: #a94442;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-error .form-control:focus {
  border-color: #843534;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #ce8483;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #ce8483;
}
.has-error .input-group-addon {
  color: #a94442;
  border-color: #a94442;
  background-color: #f2dede;
}
.has-error .form-control-feedback {
  color: #a94442;
}
.has-feedback label ~ .form-control-feedback {
  top: 23px;
}
.has-feedback label.sr-only ~ .form-control-feedback {
  top: 0;
}
.help-block {
  display: block;
  margin-top: 5px;
  margin-bottom: 10px;
  color: #404040;
}
@media (min-width: 768px) {
  .form-inline .form-group {
    display: inline-block;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .form-control {
    display: inline-block;
    width: auto;
    vertical-align: middle;
  }
  .form-inline .form-control-static {
    display: inline-block;
  }
  .form-inline .input-group {
    display: inline-table;
    vertical-align: middle;
  }
  .form-inline .input-group .input-group-addon,
  .form-inline .input-group .input-group-btn,
  .form-inline .input-group .form-control {
    width: auto;
  }
  .form-inline .input-group > .form-control {
    width: 100%;
  }
  .form-inline .control-label {
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .radio,
  .form-inline .checkbox {
    display: inline-block;
    margin-top: 0;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .radio label,
  .form-inline .checkbox label {
    padding-left: 0;
  }
  .form-inline .radio input[type="radio"],
  .form-inline .checkbox input[type="checkbox"] {
    position: relative;
    margin-left: 0;
  }
  .form-inline .has-feedback .form-control-feedback {
    top: 0;
  }
}
.form-horizontal .radio,
.form-horizontal .checkbox,
.form-horizontal .radio-inline,
.form-horizontal .checkbox-inline {
  margin-top: 0;
  margin-bottom: 0;
  padding-top: 7px;
}
.form-horizontal .radio,
.form-horizontal .checkbox {
  min-height: 25px;
}
.form-horizontal .form-group {
  margin-left: 0px;
  margin-right: 0px;
}
@media (min-width: 768px) {
  .form-horizontal .control-label {
    text-align: right;
    margin-bottom: 0;
    padding-top: 7px;
  }
}
.form-horizontal .has-feedback .form-control-feedback {
  right: 0px;
}
@media (min-width: 768px) {
  .form-horizontal .form-group-lg .control-label {
    padding-top: 11px;
    font-size: 17px;
  }
}
@media (min-width: 768px) {
  .form-horizontal .form-group-sm .control-label {
    padding-top: 6px;
    font-size: 12px;
  }
}
.btn {
  display: inline-block;
  margin-bottom: 0;
  font-weight: normal;
  text-align: center;
  vertical-align: middle;
  touch-action: manipulation;
  cursor: pointer;
  background-image: none;
  border: 1px solid transparent;
  white-space: nowrap;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  border-radius: 2px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}
.btn:focus,
.btn:active:focus,
.btn.active:focus,
.btn.focus,
.btn:active.focus,
.btn.active.focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
.btn:hover,
.btn:focus,
.btn.focus {
  color: #333;
  text-decoration: none;
}
.btn:active,
.btn.active {
  outline: 0;
  background-image: none;
  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
  box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
}
.btn.disabled,
.btn[disabled],
fieldset[disabled] .btn {
  cursor: not-allowed;
  opacity: 0.65;
  filter: alpha(opacity=65);
  -webkit-box-shadow: none;
  box-shadow: none;
}
a.btn.disabled,
fieldset[disabled] a.btn {
  pointer-events: none;
}
.btn-default {
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
.btn-default:focus,
.btn-default.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
.btn-default:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.btn-default:active,
.btn-default.active,
.open > .dropdown-toggle.btn-default {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.btn-default:active:hover,
.btn-default.active:hover,
.open > .dropdown-toggle.btn-default:hover,
.btn-default:active:focus,
.btn-default.active:focus,
.open > .dropdown-toggle.btn-default:focus,
.btn-default:active.focus,
.btn-default.active.focus,
.open > .dropdown-toggle.btn-default.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
.btn-default:active,
.btn-default.active,
.open > .dropdown-toggle.btn-default {
  background-image: none;
}
.btn-default.disabled:hover,
.btn-default[disabled]:hover,
fieldset[disabled] .btn-default:hover,
.btn-default.disabled:focus,
.btn-default[disabled]:focus,
fieldset[disabled] .btn-default:focus,
.btn-default.disabled.focus,
.btn-default[disabled].focus,
fieldset[disabled] .btn-default.focus {
  background-color: #fff;
  border-color: #ccc;
}
.btn-default .badge {
  color: #fff;
  background-color: #333;
}
.btn-primary {
  color: #fff;
  background-color: #337ab7;
  border-color: #2e6da4;
}
.btn-primary:focus,
.btn-primary.focus {
  color: #fff;
  background-color: #286090;
  border-color: #122b40;
}
.btn-primary:hover {
  color: #fff;
  background-color: #286090;
  border-color: #204d74;
}
.btn-primary:active,
.btn-primary.active,
.open > .dropdown-toggle.btn-primary {
  color: #fff;
  background-color: #286090;
  border-color: #204d74;
}
.btn-primary:active:hover,
.btn-primary.active:hover,
.open > .dropdown-toggle.btn-primary:hover,
.btn-primary:active:focus,
.btn-primary.active:focus,
.open > .dropdown-toggle.btn-primary:focus,
.btn-primary:active.focus,
.btn-primary.active.focus,
.open > .dropdown-toggle.btn-primary.focus {
  color: #fff;
  background-color: #204d74;
  border-color: #122b40;
}
.btn-primary:active,
.btn-primary.active,
.open > .dropdown-toggle.btn-primary {
  background-image: none;
}
.btn-primary.disabled:hover,
.btn-primary[disabled]:hover,
fieldset[disabled] .btn-primary:hover,
.btn-primary.disabled:focus,
.btn-primary[disabled]:focus,
fieldset[disabled] .btn-primary:focus,
.btn-primary.disabled.focus,
.btn-primary[disabled].focus,
fieldset[disabled] .btn-primary.focus {
  background-color: #337ab7;
  border-color: #2e6da4;
}
.btn-primary .badge {
  color: #337ab7;
  background-color: #fff;
}
.btn-success {
  color: #fff;
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.btn-success:focus,
.btn-success.focus {
  color: #fff;
  background-color: #449d44;
  border-color: #255625;
}
.btn-success:hover {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.btn-success:active,
.btn-success.active,
.open > .dropdown-toggle.btn-success {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.btn-success:active:hover,
.btn-success.active:hover,
.open > .dropdown-toggle.btn-success:hover,
.btn-success:active:focus,
.btn-success.active:focus,
.open > .dropdown-toggle.btn-success:focus,
.btn-success:active.focus,
.btn-success.active.focus,
.open > .dropdown-toggle.btn-success.focus {
  color: #fff;
  background-color: #398439;
  border-color: #255625;
}
.btn-success:active,
.btn-success.active,
.open > .dropdown-toggle.btn-success {
  background-image: none;
}
.btn-success.disabled:hover,
.btn-success[disabled]:hover,
fieldset[disabled] .btn-success:hover,
.btn-success.disabled:focus,
.btn-success[disabled]:focus,
fieldset[disabled] .btn-success:focus,
.btn-success.disabled.focus,
.btn-success[disabled].focus,
fieldset[disabled] .btn-success.focus {
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.btn-success .badge {
  color: #5cb85c;
  background-color: #fff;
}
.btn-info {
  color: #fff;
  background-color: #5bc0de;
  border-color: #46b8da;
}
.btn-info:focus,
.btn-info.focus {
  color: #fff;
  background-color: #31b0d5;
  border-color: #1b6d85;
}
.btn-info:hover {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.btn-info:active,
.btn-info.active,
.open > .dropdown-toggle.btn-info {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.btn-info:active:hover,
.btn-info.active:hover,
.open > .dropdown-toggle.btn-info:hover,
.btn-info:active:focus,
.btn-info.active:focus,
.open > .dropdown-toggle.btn-info:focus,
.btn-info:active.focus,
.btn-info.active.focus,
.open > .dropdown-toggle.btn-info.focus {
  color: #fff;
  background-color: #269abc;
  border-color: #1b6d85;
}
.btn-info:active,
.btn-info.active,
.open > .dropdown-toggle.btn-info {
  background-image: none;
}
.btn-info.disabled:hover,
.btn-info[disabled]:hover,
fieldset[disabled] .btn-info:hover,
.btn-info.disabled:focus,
.btn-info[disabled]:focus,
fieldset[disabled] .btn-info:focus,
.btn-info.disabled.focus,
.btn-info[disabled].focus,
fieldset[disabled] .btn-info.focus {
  background-color: #5bc0de;
  border-color: #46b8da;
}
.btn-info .badge {
  color: #5bc0de;
  background-color: #fff;
}
.btn-warning {
  color: #fff;
  background-color: #f0ad4e;
  border-color: #eea236;
}
.btn-warning:focus,
.btn-warning.focus {
  color: #fff;
  background-color: #ec971f;
  border-color: #985f0d;
}
.btn-warning:hover {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.btn-warning:active,
.btn-warning.active,
.open > .dropdown-toggle.btn-warning {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.btn-warning:active:hover,
.btn-warning.active:hover,
.open > .dropdown-toggle.btn-warning:hover,
.btn-warning:active:focus,
.btn-warning.active:focus,
.open > .dropdown-toggle.btn-warning:focus,
.btn-warning:active.focus,
.btn-warning.active.focus,
.open > .dropdown-toggle.btn-warning.focus {
  color: #fff;
  background-color: #d58512;
  border-color: #985f0d;
}
.btn-warning:active,
.btn-warning.active,
.open > .dropdown-toggle.btn-warning {
  background-image: none;
}
.btn-warning.disabled:hover,
.btn-warning[disabled]:hover,
fieldset[disabled] .btn-warning:hover,
.btn-warning.disabled:focus,
.btn-warning[disabled]:focus,
fieldset[disabled] .btn-warning:focus,
.btn-warning.disabled.focus,
.btn-warning[disabled].focus,
fieldset[disabled] .btn-warning.focus {
  background-color: #f0ad4e;
  border-color: #eea236;
}
.btn-warning .badge {
  color: #f0ad4e;
  background-color: #fff;
}
.btn-danger {
  color: #fff;
  background-color: #d9534f;
  border-color: #d43f3a;
}
.btn-danger:focus,
.btn-danger.focus {
  color: #fff;
  background-color: #c9302c;
  border-color: #761c19;
}
.btn-danger:hover {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.btn-danger:active,
.btn-danger.active,
.open > .dropdown-toggle.btn-danger {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.btn-danger:active:hover,
.btn-danger.active:hover,
.open > .dropdown-toggle.btn-danger:hover,
.btn-danger:active:focus,
.btn-danger.active:focus,
.open > .dropdown-toggle.btn-danger:focus,
.btn-danger:active.focus,
.btn-danger.active.focus,
.open > .dropdown-toggle.btn-danger.focus {
  color: #fff;
  background-color: #ac2925;
  border-color: #761c19;
}
.btn-danger:active,
.btn-danger.active,
.open > .dropdown-toggle.btn-danger {
  background-image: none;
}
.btn-danger.disabled:hover,
.btn-danger[disabled]:hover,
fieldset[disabled] .btn-danger:hover,
.btn-danger.disabled:focus,
.btn-danger[disabled]:focus,
fieldset[disabled] .btn-danger:focus,
.btn-danger.disabled.focus,
.btn-danger[disabled].focus,
fieldset[disabled] .btn-danger.focus {
  background-color: #d9534f;
  border-color: #d43f3a;
}
.btn-danger .badge {
  color: #d9534f;
  background-color: #fff;
}
.btn-link {
  color: #337ab7;
  font-weight: normal;
  border-radius: 0;
}
.btn-link,
.btn-link:active,
.btn-link.active,
.btn-link[disabled],
fieldset[disabled] .btn-link {
  background-color: transparent;
  -webkit-box-shadow: none;
  box-shadow: none;
}
.btn-link,
.btn-link:hover,
.btn-link:focus,
.btn-link:active {
  border-color: transparent;
}
.btn-link:hover,
.btn-link:focus {
  color: #23527c;
  text-decoration: underline;
  background-color: transparent;
}
.btn-link[disabled]:hover,
fieldset[disabled] .btn-link:hover,
.btn-link[disabled]:focus,
fieldset[disabled] .btn-link:focus {
  color: #777777;
  text-decoration: none;
}
.btn-lg,
.btn-group-lg > .btn {
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
.btn-sm,
.btn-group-sm > .btn {
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.btn-xs,
.btn-group-xs > .btn {
  padding: 1px 5px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.btn-block {
  display: block;
  width: 100%;
}
.btn-block + .btn-block {
  margin-top: 5px;
}
input[type="submit"].btn-block,
input[type="reset"].btn-block,
input[type="button"].btn-block {
  width: 100%;
}
.fade {
  opacity: 0;
  -webkit-transition: opacity 0.15s linear;
  -o-transition: opacity 0.15s linear;
  transition: opacity 0.15s linear;
}
.fade.in {
  opacity: 1;
}
.collapse {
  display: none;
}
.collapse.in {
  display: block;
}
tr.collapse.in {
  display: table-row;
}
tbody.collapse.in {
  display: table-row-group;
}
.collapsing {
  position: relative;
  height: 0;
  overflow: hidden;
  -webkit-transition-property: height, visibility;
  transition-property: height, visibility;
  -webkit-transition-duration: 0.35s;
  transition-duration: 0.35s;
  -webkit-transition-timing-function: ease;
  transition-timing-function: ease;
}
.caret {
  display: inline-block;
  width: 0;
  height: 0;
  margin-left: 2px;
  vertical-align: middle;
  border-top: 4px dashed;
  border-top: 4px solid \9;
  border-right: 4px solid transparent;
  border-left: 4px solid transparent;
}
.dropup,
.dropdown {
  position: relative;
}
.dropdown-toggle:focus {
  outline: 0;
}
.dropdown-menu {
  position: absolute;
  top: 100%;
  left: 0;
  z-index: 1000;
  display: none;
  float: left;
  min-width: 160px;
  padding: 5px 0;
  margin: 2px 0 0;
  list-style: none;
  font-size: 13px;
  text-align: left;
  background-color: #fff;
  border: 1px solid #ccc;
  border: 1px solid rgba(0, 0, 0, 0.15);
  border-radius: 2px;
  -webkit-box-shadow: 0 6px 12px rgba(0, 0, 0, 0.175);
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.175);
  background-clip: padding-box;
}
.dropdown-menu.pull-right {
  right: 0;
  left: auto;
}
.dropdown-menu .divider {
  height: 1px;
  margin: 8px 0;
  overflow: hidden;
  background-color: #e5e5e5;
}
.dropdown-menu > li > a {
  display: block;
  padding: 3px 20px;
  clear: both;
  font-weight: normal;
  line-height: 1.42857143;
  color: #333333;
  white-space: nowrap;
}
.dropdown-menu > li > a:hover,
.dropdown-menu > li > a:focus {
  text-decoration: none;
  color: #262626;
  background-color: #f5f5f5;
}
.dropdown-menu > .active > a,
.dropdown-menu > .active > a:hover,
.dropdown-menu > .active > a:focus {
  color: #fff;
  text-decoration: none;
  outline: 0;
  background-color: #337ab7;
}
.dropdown-menu > .disabled > a,
.dropdown-menu > .disabled > a:hover,
.dropdown-menu > .disabled > a:focus {
  color: #777777;
}
.dropdown-menu > .disabled > a:hover,
.dropdown-menu > .disabled > a:focus {
  text-decoration: none;
  background-color: transparent;
  background-image: none;
  filter: progid:DXImageTransform.Microsoft.gradient(enabled = false);
  cursor: not-allowed;
}
.open > .dropdown-menu {
  display: block;
}
.open > a {
  outline: 0;
}
.dropdown-menu-right {
  left: auto;
  right: 0;
}
.dropdown-menu-left {
  left: 0;
  right: auto;
}
.dropdown-header {
  display: block;
  padding: 3px 20px;
  font-size: 12px;
  line-height: 1.42857143;
  color: #777777;
  white-space: nowrap;
}
.dropdown-backdrop {
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  top: 0;
  z-index: 990;
}
.pull-right > .dropdown-menu {
  right: 0;
  left: auto;
}
.dropup .caret,
.navbar-fixed-bottom .dropdown .caret {
  border-top: 0;
  border-bottom: 4px dashed;
  border-bottom: 4px solid \9;
  content: "";
}
.dropup .dropdown-menu,
.navbar-fixed-bottom .dropdown .dropdown-menu {
  top: auto;
  bottom: 100%;
  margin-bottom: 2px;
}
@media (min-width: 541px) {
  .navbar-right .dropdown-menu {
    left: auto;
    right: 0;
  }
  .navbar-right .dropdown-menu-left {
    left: 0;
    right: auto;
  }
}
.btn-group,
.btn-group-vertical {
  position: relative;
  display: inline-block;
  vertical-align: middle;
}
.btn-group > .btn,
.btn-group-vertical > .btn {
  position: relative;
  float: left;
}
.btn-group > .btn:hover,
.btn-group-vertical > .btn:hover,
.btn-group > .btn:focus,
.btn-group-vertical > .btn:focus,
.btn-group > .btn:active,
.btn-group-vertical > .btn:active,
.btn-group > .btn.active,
.btn-group-vertical > .btn.active {
  z-index: 2;
}
.btn-group .btn + .btn,
.btn-group .btn + .btn-group,
.btn-group .btn-group + .btn,
.btn-group .btn-group + .btn-group {
  margin-left: -1px;
}
.btn-toolbar {
  margin-left: -5px;
}
.btn-toolbar .btn,
.btn-toolbar .btn-group,
.btn-toolbar .input-group {
  float: left;
}
.btn-toolbar > .btn,
.btn-toolbar > .btn-group,
.btn-toolbar > .input-group {
  margin-left: 5px;
}
.btn-group > .btn:not(:first-child):not(:last-child):not(.dropdown-toggle) {
  border-radius: 0;
}
.btn-group > .btn:first-child {
  margin-left: 0;
}
.btn-group > .btn:first-child:not(:last-child):not(.dropdown-toggle) {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.btn-group > .btn:last-child:not(:first-child),
.btn-group > .dropdown-toggle:not(:first-child) {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.btn-group > .btn-group {
  float: left;
}
.btn-group > .btn-group:not(:first-child):not(:last-child) > .btn {
  border-radius: 0;
}
.btn-group > .btn-group:first-child:not(:last-child) > .btn:last-child,
.btn-group > .btn-group:first-child:not(:last-child) > .dropdown-toggle {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.btn-group > .btn-group:last-child:not(:first-child) > .btn:first-child {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.btn-group .dropdown-toggle:active,
.btn-group.open .dropdown-toggle {
  outline: 0;
}
.btn-group > .btn + .dropdown-toggle {
  padding-left: 8px;
  padding-right: 8px;
}
.btn-group > .btn-lg + .dropdown-toggle {
  padding-left: 12px;
  padding-right: 12px;
}
.btn-group.open .dropdown-toggle {
  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
  box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
}
.btn-group.open .dropdown-toggle.btn-link {
  -webkit-box-shadow: none;
  box-shadow: none;
}
.btn .caret {
  margin-left: 0;
}
.btn-lg .caret {
  border-width: 5px 5px 0;
  border-bottom-width: 0;
}
.dropup .btn-lg .caret {
  border-width: 0 5px 5px;
}
.btn-group-vertical > .btn,
.btn-group-vertical > .btn-group,
.btn-group-vertical > .btn-group > .btn {
  display: block;
  float: none;
  width: 100%;
  max-width: 100%;
}
.btn-group-vertical > .btn-group > .btn {
  float: none;
}
.btn-group-vertical > .btn + .btn,
.btn-group-vertical > .btn + .btn-group,
.btn-group-vertical > .btn-group + .btn,
.btn-group-vertical > .btn-group + .btn-group {
  margin-top: -1px;
  margin-left: 0;
}
.btn-group-vertical > .btn:not(:first-child):not(:last-child) {
  border-radius: 0;
}
.btn-group-vertical > .btn:first-child:not(:last-child) {
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.btn-group-vertical > .btn:last-child:not(:first-child) {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
  border-bottom-right-radius: 2px;
  border-bottom-left-radius: 2px;
}
.btn-group-vertical > .btn-group:not(:first-child):not(:last-child) > .btn {
  border-radius: 0;
}
.btn-group-vertical > .btn-group:first-child:not(:last-child) > .btn:last-child,
.btn-group-vertical > .btn-group:first-child:not(:last-child) > .dropdown-toggle {
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.btn-group-vertical > .btn-group:last-child:not(:first-child) > .btn:first-child {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.btn-group-justified {
  display: table;
  width: 100%;
  table-layout: fixed;
  border-collapse: separate;
}
.btn-group-justified > .btn,
.btn-group-justified > .btn-group {
  float: none;
  display: table-cell;
  width: 1%;
}
.btn-group-justified > .btn-group .btn {
  width: 100%;
}
.btn-group-justified > .btn-group .dropdown-menu {
  left: auto;
}
[data-toggle="buttons"] > .btn input[type="radio"],
[data-toggle="buttons"] > .btn-group > .btn input[type="radio"],
[data-toggle="buttons"] > .btn input[type="checkbox"],
[data-toggle="buttons"] > .btn-group > .btn input[type="checkbox"] {
  position: absolute;
  clip: rect(0, 0, 0, 0);
  pointer-events: none;
}
.input-group {
  position: relative;
  display: table;
  border-collapse: separate;
}
.input-group[class*="col-"] {
  float: none;
  padding-left: 0;
  padding-right: 0;
}
.input-group .form-control {
  position: relative;
  z-index: 2;
  float: left;
  width: 100%;
  margin-bottom: 0;
}
.input-group .form-control:focus {
  z-index: 3;
}
.input-group-lg > .form-control,
.input-group-lg > .input-group-addon,
.input-group-lg > .input-group-btn > .btn {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
select.input-group-lg > .form-control,
select.input-group-lg > .input-group-addon,
select.input-group-lg > .input-group-btn > .btn {
  height: 45px;
  line-height: 45px;
}
textarea.input-group-lg > .form-control,
textarea.input-group-lg > .input-group-addon,
textarea.input-group-lg > .input-group-btn > .btn,
select[multiple].input-group-lg > .form-control,
select[multiple].input-group-lg > .input-group-addon,
select[multiple].input-group-lg > .input-group-btn > .btn {
  height: auto;
}
.input-group-sm > .form-control,
.input-group-sm > .input-group-addon,
.input-group-sm > .input-group-btn > .btn {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
select.input-group-sm > .form-control,
select.input-group-sm > .input-group-addon,
select.input-group-sm > .input-group-btn > .btn {
  height: 30px;
  line-height: 30px;
}
textarea.input-group-sm > .form-control,
textarea.input-group-sm > .input-group-addon,
textarea.input-group-sm > .input-group-btn > .btn,
select[multiple].input-group-sm > .form-control,
select[multiple].input-group-sm > .input-group-addon,
select[multiple].input-group-sm > .input-group-btn > .btn {
  height: auto;
}
.input-group-addon,
.input-group-btn,
.input-group .form-control {
  display: table-cell;
}
.input-group-addon:not(:first-child):not(:last-child),
.input-group-btn:not(:first-child):not(:last-child),
.input-group .form-control:not(:first-child):not(:last-child) {
  border-radius: 0;
}
.input-group-addon,
.input-group-btn {
  width: 1%;
  white-space: nowrap;
  vertical-align: middle;
}
.input-group-addon {
  padding: 6px 12px;
  font-size: 13px;
  font-weight: normal;
  line-height: 1;
  color: #555555;
  text-align: center;
  background-color: #eeeeee;
  border: 1px solid #ccc;
  border-radius: 2px;
}
.input-group-addon.input-sm {
  padding: 5px 10px;
  font-size: 12px;
  border-radius: 1px;
}
.input-group-addon.input-lg {
  padding: 10px 16px;
  font-size: 17px;
  border-radius: 3px;
}
.input-group-addon input[type="radio"],
.input-group-addon input[type="checkbox"] {
  margin-top: 0;
}
.input-group .form-control:first-child,
.input-group-addon:first-child,
.input-group-btn:first-child > .btn,
.input-group-btn:first-child > .btn-group > .btn,
.input-group-btn:first-child > .dropdown-toggle,
.input-group-btn:last-child > .btn:not(:last-child):not(.dropdown-toggle),
.input-group-btn:last-child > .btn-group:not(:last-child) > .btn {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.input-group-addon:first-child {
  border-right: 0;
}
.input-group .form-control:last-child,
.input-group-addon:last-child,
.input-group-btn:last-child > .btn,
.input-group-btn:last-child > .btn-group > .btn,
.input-group-btn:last-child > .dropdown-toggle,
.input-group-btn:first-child > .btn:not(:first-child),
.input-group-btn:first-child > .btn-group:not(:first-child) > .btn {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.input-group-addon:last-child {
  border-left: 0;
}
.input-group-btn {
  position: relative;
  font-size: 0;
  white-space: nowrap;
}
.input-group-btn > .btn {
  position: relative;
}
.input-group-btn > .btn + .btn {
  margin-left: -1px;
}
.input-group-btn > .btn:hover,
.input-group-btn > .btn:focus,
.input-group-btn > .btn:active {
  z-index: 2;
}
.input-group-btn:first-child > .btn,
.input-group-btn:first-child > .btn-group {
  margin-right: -1px;
}
.input-group-btn:last-child > .btn,
.input-group-btn:last-child > .btn-group {
  z-index: 2;
  margin-left: -1px;
}
.nav {
  margin-bottom: 0;
  padding-left: 0;
  list-style: none;
}
.nav > li {
  position: relative;
  display: block;
}
.nav > li > a {
  position: relative;
  display: block;
  padding: 10px 15px;
}
.nav > li > a:hover,
.nav > li > a:focus {
  text-decoration: none;
  background-color: #eeeeee;
}
.nav > li.disabled > a {
  color: #777777;
}
.nav > li.disabled > a:hover,
.nav > li.disabled > a:focus {
  color: #777777;
  text-decoration: none;
  background-color: transparent;
  cursor: not-allowed;
}
.nav .open > a,
.nav .open > a:hover,
.nav .open > a:focus {
  background-color: #eeeeee;
  border-color: #337ab7;
}
.nav .nav-divider {
  height: 1px;
  margin: 8px 0;
  overflow: hidden;
  background-color: #e5e5e5;
}
.nav > li > a > img {
  max-width: none;
}
.nav-tabs {
  border-bottom: 1px solid #ddd;
}
.nav-tabs > li {
  float: left;
  margin-bottom: -1px;
}
.nav-tabs > li > a {
  margin-right: 2px;
  line-height: 1.42857143;
  border: 1px solid transparent;
  border-radius: 2px 2px 0 0;
}
.nav-tabs > li > a:hover {
  border-color: #eeeeee #eeeeee #ddd;
}
.nav-tabs > li.active > a,
.nav-tabs > li.active > a:hover,
.nav-tabs > li.active > a:focus {
  color: #555555;
  background-color: #fff;
  border: 1px solid #ddd;
  border-bottom-color: transparent;
  cursor: default;
}
.nav-tabs.nav-justified {
  width: 100%;
  border-bottom: 0;
}
.nav-tabs.nav-justified > li {
  float: none;
}
.nav-tabs.nav-justified > li > a {
  text-align: center;
  margin-bottom: 5px;
}
.nav-tabs.nav-justified > .dropdown .dropdown-menu {
  top: auto;
  left: auto;
}
@media (min-width: 768px) {
  .nav-tabs.nav-justified > li {
    display: table-cell;
    width: 1%;
  }
  .nav-tabs.nav-justified > li > a {
    margin-bottom: 0;
  }
}
.nav-tabs.nav-justified > li > a {
  margin-right: 0;
  border-radius: 2px;
}
.nav-tabs.nav-justified > .active > a,
.nav-tabs.nav-justified > .active > a:hover,
.nav-tabs.nav-justified > .active > a:focus {
  border: 1px solid #ddd;
}
@media (min-width: 768px) {
  .nav-tabs.nav-justified > li > a {
    border-bottom: 1px solid #ddd;
    border-radius: 2px 2px 0 0;
  }
  .nav-tabs.nav-justified > .active > a,
  .nav-tabs.nav-justified > .active > a:hover,
  .nav-tabs.nav-justified > .active > a:focus {
    border-bottom-color: #fff;
  }
}
.nav-pills > li {
  float: left;
}
.nav-pills > li > a {
  border-radius: 2px;
}
.nav-pills > li + li {
  margin-left: 2px;
}
.nav-pills > li.active > a,
.nav-pills > li.active > a:hover,
.nav-pills > li.active > a:focus {
  color: #fff;
  background-color: #337ab7;
}
.nav-stacked > li {
  float: none;
}
.nav-stacked > li + li {
  margin-top: 2px;
  margin-left: 0;
}
.nav-justified {
  width: 100%;
}
.nav-justified > li {
  float: none;
}
.nav-justified > li > a {
  text-align: center;
  margin-bottom: 5px;
}
.nav-justified > .dropdown .dropdown-menu {
  top: auto;
  left: auto;
}
@media (min-width: 768px) {
  .nav-justified > li {
    display: table-cell;
    width: 1%;
  }
  .nav-justified > li > a {
    margin-bottom: 0;
  }
}
.nav-tabs-justified {
  border-bottom: 0;
}
.nav-tabs-justified > li > a {
  margin-right: 0;
  border-radius: 2px;
}
.nav-tabs-justified > .active > a,
.nav-tabs-justified > .active > a:hover,
.nav-tabs-justified > .active > a:focus {
  border: 1px solid #ddd;
}
@media (min-width: 768px) {
  .nav-tabs-justified > li > a {
    border-bottom: 1px solid #ddd;
    border-radius: 2px 2px 0 0;
  }
  .nav-tabs-justified > .active > a,
  .nav-tabs-justified > .active > a:hover,
  .nav-tabs-justified > .active > a:focus {
    border-bottom-color: #fff;
  }
}
.tab-content > .tab-pane {
  display: none;
}
.tab-content > .active {
  display: block;
}
.nav-tabs .dropdown-menu {
  margin-top: -1px;
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.navbar {
  position: relative;
  min-height: 30px;
  margin-bottom: 18px;
  border: 1px solid transparent;
}
@media (min-width: 541px) {
  .navbar {
    border-radius: 2px;
  }
}
@media (min-width: 541px) {
  .navbar-header {
    float: left;
  }
}
.navbar-collapse {
  overflow-x: visible;
  padding-right: 0px;
  padding-left: 0px;
  border-top: 1px solid transparent;
  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1);
  -webkit-overflow-scrolling: touch;
}
.navbar-collapse.in {
  overflow-y: auto;
}
@media (min-width: 541px) {
  .navbar-collapse {
    width: auto;
    border-top: 0;
    box-shadow: none;
  }
  .navbar-collapse.collapse {
    display: block !important;
    height: auto !important;
    padding-bottom: 0;
    overflow: visible !important;
  }
  .navbar-collapse.in {
    overflow-y: visible;
  }
  .navbar-fixed-top .navbar-collapse,
  .navbar-static-top .navbar-collapse,
  .navbar-fixed-bottom .navbar-collapse {
    padding-left: 0;
    padding-right: 0;
  }
}
.navbar-fixed-top .navbar-collapse,
.navbar-fixed-bottom .navbar-collapse {
  max-height: 340px;
}
@media (max-device-width: 540px) and (orientation: landscape) {
  .navbar-fixed-top .navbar-collapse,
  .navbar-fixed-bottom .navbar-collapse {
    max-height: 200px;
  }
}
.container > .navbar-header,
.container-fluid > .navbar-header,
.container > .navbar-collapse,
.container-fluid > .navbar-collapse {
  margin-right: 0px;
  margin-left: 0px;
}
@media (min-width: 541px) {
  .container > .navbar-header,
  .container-fluid > .navbar-header,
  .container > .navbar-collapse,
  .container-fluid > .navbar-collapse {
    margin-right: 0;
    margin-left: 0;
  }
}
.navbar-static-top {
  z-index: 1000;
  border-width: 0 0 1px;
}
@media (min-width: 541px) {
  .navbar-static-top {
    border-radius: 0;
  }
}
.navbar-fixed-top,
.navbar-fixed-bottom {
  position: fixed;
  right: 0;
  left: 0;
  z-index: 1030;
}
@media (min-width: 541px) {
  .navbar-fixed-top,
  .navbar-fixed-bottom {
    border-radius: 0;
  }
}
.navbar-fixed-top {
  top: 0;
  border-width: 0 0 1px;
}
.navbar-fixed-bottom {
  bottom: 0;
  margin-bottom: 0;
  border-width: 1px 0 0;
}
.navbar-brand {
  float: left;
  padding: 6px 0px;
  font-size: 17px;
  line-height: 18px;
  height: 30px;
}
.navbar-brand:hover,
.navbar-brand:focus {
  text-decoration: none;
}
.navbar-brand > img {
  display: block;
}
@media (min-width: 541px) {
  .navbar > .container .navbar-brand,
  .navbar > .container-fluid .navbar-brand {
    margin-left: 0px;
  }
}
.navbar-toggle {
  position: relative;
  float: right;
  margin-right: 0px;
  padding: 9px 10px;
  margin-top: -2px;
  margin-bottom: -2px;
  background-color: transparent;
  background-image: none;
  border: 1px solid transparent;
  border-radius: 2px;
}
.navbar-toggle:focus {
  outline: 0;
}
.navbar-toggle .icon-bar {
  display: block;
  width: 22px;
  height: 2px;
  border-radius: 1px;
}
.navbar-toggle .icon-bar + .icon-bar {
  margin-top: 4px;
}
@media (min-width: 541px) {
  .navbar-toggle {
    display: none;
  }
}
.navbar-nav {
  margin: 3px 0px;
}
.navbar-nav > li > a {
  padding-top: 10px;
  padding-bottom: 10px;
  line-height: 18px;
}
@media (max-width: 540px) {
  .navbar-nav .open .dropdown-menu {
    position: static;
    float: none;
    width: auto;
    margin-top: 0;
    background-color: transparent;
    border: 0;
    box-shadow: none;
  }
  .navbar-nav .open .dropdown-menu > li > a,
  .navbar-nav .open .dropdown-menu .dropdown-header {
    padding: 5px 15px 5px 25px;
  }
  .navbar-nav .open .dropdown-menu > li > a {
    line-height: 18px;
  }
  .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-nav .open .dropdown-menu > li > a:focus {
    background-image: none;
  }
}
@media (min-width: 541px) {
  .navbar-nav {
    float: left;
    margin: 0;
  }
  .navbar-nav > li {
    float: left;
  }
  .navbar-nav > li > a {
    padding-top: 6px;
    padding-bottom: 6px;
  }
}
.navbar-form {
  margin-left: 0px;
  margin-right: 0px;
  padding: 10px 0px;
  border-top: 1px solid transparent;
  border-bottom: 1px solid transparent;
  -webkit-box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1), 0 1px 0 rgba(255, 255, 255, 0.1);
  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1), 0 1px 0 rgba(255, 255, 255, 0.1);
  margin-top: -1px;
  margin-bottom: -1px;
}
@media (min-width: 768px) {
  .navbar-form .form-group {
    display: inline-block;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .form-control {
    display: inline-block;
    width: auto;
    vertical-align: middle;
  }
  .navbar-form .form-control-static {
    display: inline-block;
  }
  .navbar-form .input-group {
    display: inline-table;
    vertical-align: middle;
  }
  .navbar-form .input-group .input-group-addon,
  .navbar-form .input-group .input-group-btn,
  .navbar-form .input-group .form-control {
    width: auto;
  }
  .navbar-form .input-group > .form-control {
    width: 100%;
  }
  .navbar-form .control-label {
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .radio,
  .navbar-form .checkbox {
    display: inline-block;
    margin-top: 0;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .radio label,
  .navbar-form .checkbox label {
    padding-left: 0;
  }
  .navbar-form .radio input[type="radio"],
  .navbar-form .checkbox input[type="checkbox"] {
    position: relative;
    margin-left: 0;
  }
  .navbar-form .has-feedback .form-control-feedback {
    top: 0;
  }
}
@media (max-width: 540px) {
  .navbar-form .form-group {
    margin-bottom: 5px;
  }
  .navbar-form .form-group:last-child {
    margin-bottom: 0;
  }
}
@media (min-width: 541px) {
  .navbar-form {
    width: auto;
    border: 0;
    margin-left: 0;
    margin-right: 0;
    padding-top: 0;
    padding-bottom: 0;
    -webkit-box-shadow: none;
    box-shadow: none;
  }
}
.navbar-nav > li > .dropdown-menu {
  margin-top: 0;
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.navbar-fixed-bottom .navbar-nav > li > .dropdown-menu {
  margin-bottom: 0;
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.navbar-btn {
  margin-top: -1px;
  margin-bottom: -1px;
}
.navbar-btn.btn-sm {
  margin-top: 0px;
  margin-bottom: 0px;
}
.navbar-btn.btn-xs {
  margin-top: 4px;
  margin-bottom: 4px;
}
.navbar-text {
  margin-top: 6px;
  margin-bottom: 6px;
}
@media (min-width: 541px) {
  .navbar-text {
    float: left;
    margin-left: 0px;
    margin-right: 0px;
  }
}
@media (min-width: 541px) {
  .navbar-left {
    float: left !important;
    float: left;
  }
  .navbar-right {
    float: right !important;
    float: right;
    margin-right: 0px;
  }
  .navbar-right ~ .navbar-right {
    margin-right: 0;
  }
}
.navbar-default {
  background-color: #f8f8f8;
  border-color: #e7e7e7;
}
.navbar-default .navbar-brand {
  color: #777;
}
.navbar-default .navbar-brand:hover,
.navbar-default .navbar-brand:focus {
  color: #5e5e5e;
  background-color: transparent;
}
.navbar-default .navbar-text {
  color: #777;
}
.navbar-default .navbar-nav > li > a {
  color: #777;
}
.navbar-default .navbar-nav > li > a:hover,
.navbar-default .navbar-nav > li > a:focus {
  color: #333;
  background-color: transparent;
}
.navbar-default .navbar-nav > .active > a,
.navbar-default .navbar-nav > .active > a:hover,
.navbar-default .navbar-nav > .active > a:focus {
  color: #555;
  background-color: #e7e7e7;
}
.navbar-default .navbar-nav > .disabled > a,
.navbar-default .navbar-nav > .disabled > a:hover,
.navbar-default .navbar-nav > .disabled > a:focus {
  color: #ccc;
  background-color: transparent;
}
.navbar-default .navbar-toggle {
  border-color: #ddd;
}
.navbar-default .navbar-toggle:hover,
.navbar-default .navbar-toggle:focus {
  background-color: #ddd;
}
.navbar-default .navbar-toggle .icon-bar {
  background-color: #888;
}
.navbar-default .navbar-collapse,
.navbar-default .navbar-form {
  border-color: #e7e7e7;
}
.navbar-default .navbar-nav > .open > a,
.navbar-default .navbar-nav > .open > a:hover,
.navbar-default .navbar-nav > .open > a:focus {
  background-color: #e7e7e7;
  color: #555;
}
@media (max-width: 540px) {
  .navbar-default .navbar-nav .open .dropdown-menu > li > a {
    color: #777;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > li > a:focus {
    color: #333;
    background-color: transparent;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a,
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a:focus {
    color: #555;
    background-color: #e7e7e7;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a,
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a:focus {
    color: #ccc;
    background-color: transparent;
  }
}
.navbar-default .navbar-link {
  color: #777;
}
.navbar-default .navbar-link:hover {
  color: #333;
}
.navbar-default .btn-link {
  color: #777;
}
.navbar-default .btn-link:hover,
.navbar-default .btn-link:focus {
  color: #333;
}
.navbar-default .btn-link[disabled]:hover,
fieldset[disabled] .navbar-default .btn-link:hover,
.navbar-default .btn-link[disabled]:focus,
fieldset[disabled] .navbar-default .btn-link:focus {
  color: #ccc;
}
.navbar-inverse {
  background-color: #222;
  border-color: #080808;
}
.navbar-inverse .navbar-brand {
  color: #9d9d9d;
}
.navbar-inverse .navbar-brand:hover,
.navbar-inverse .navbar-brand:focus {
  color: #fff;
  background-color: transparent;
}
.navbar-inverse .navbar-text {
  color: #9d9d9d;
}
.navbar-inverse .navbar-nav > li > a {
  color: #9d9d9d;
}
.navbar-inverse .navbar-nav > li > a:hover,
.navbar-inverse .navbar-nav > li > a:focus {
  color: #fff;
  background-color: transparent;
}
.navbar-inverse .navbar-nav > .active > a,
.navbar-inverse .navbar-nav > .active > a:hover,
.navbar-inverse .navbar-nav > .active > a:focus {
  color: #fff;
  background-color: #080808;
}
.navbar-inverse .navbar-nav > .disabled > a,
.navbar-inverse .navbar-nav > .disabled > a:hover,
.navbar-inverse .navbar-nav > .disabled > a:focus {
  color: #444;
  background-color: transparent;
}
.navbar-inverse .navbar-toggle {
  border-color: #333;
}
.navbar-inverse .navbar-toggle:hover,
.navbar-inverse .navbar-toggle:focus {
  background-color: #333;
}
.navbar-inverse .navbar-toggle .icon-bar {
  background-color: #fff;
}
.navbar-inverse .navbar-collapse,
.navbar-inverse .navbar-form {
  border-color: #101010;
}
.navbar-inverse .navbar-nav > .open > a,
.navbar-inverse .navbar-nav > .open > a:hover,
.navbar-inverse .navbar-nav > .open > a:focus {
  background-color: #080808;
  color: #fff;
}
@media (max-width: 540px) {
  .navbar-inverse .navbar-nav .open .dropdown-menu > .dropdown-header {
    border-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu .divider {
    background-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a {
    color: #9d9d9d;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a:focus {
    color: #fff;
    background-color: transparent;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a:focus {
    color: #fff;
    background-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a:focus {
    color: #444;
    background-color: transparent;
  }
}
.navbar-inverse .navbar-link {
  color: #9d9d9d;
}
.navbar-inverse .navbar-link:hover {
  color: #fff;
}
.navbar-inverse .btn-link {
  color: #9d9d9d;
}
.navbar-inverse .btn-link:hover,
.navbar-inverse .btn-link:focus {
  color: #fff;
}
.navbar-inverse .btn-link[disabled]:hover,
fieldset[disabled] .navbar-inverse .btn-link:hover,
.navbar-inverse .btn-link[disabled]:focus,
fieldset[disabled] .navbar-inverse .btn-link:focus {
  color: #444;
}
.breadcrumb {
  padding: 8px 15px;
  margin-bottom: 18px;
  list-style: none;
  background-color: #f5f5f5;
  border-radius: 2px;
}
.breadcrumb > li {
  display: inline-block;
}
.breadcrumb > li + li:before {
  content: "/\00a0";
  padding: 0 5px;
  color: #5e5e5e;
}
.breadcrumb > .active {
  color: #777777;
}
.pagination {
  display: inline-block;
  padding-left: 0;
  margin: 18px 0;
  border-radius: 2px;
}
.pagination > li {
  display: inline;
}
.pagination > li > a,
.pagination > li > span {
  position: relative;
  float: left;
  padding: 6px 12px;
  line-height: 1.42857143;
  text-decoration: none;
  color: #337ab7;
  background-color: #fff;
  border: 1px solid #ddd;
  margin-left: -1px;
}
.pagination > li:first-child > a,
.pagination > li:first-child > span {
  margin-left: 0;
  border-bottom-left-radius: 2px;
  border-top-left-radius: 2px;
}
.pagination > li:last-child > a,
.pagination > li:last-child > span {
  border-bottom-right-radius: 2px;
  border-top-right-radius: 2px;
}
.pagination > li > a:hover,
.pagination > li > span:hover,
.pagination > li > a:focus,
.pagination > li > span:focus {
  z-index: 2;
  color: #23527c;
  background-color: #eeeeee;
  border-color: #ddd;
}
.pagination > .active > a,
.pagination > .active > span,
.pagination > .active > a:hover,
.pagination > .active > span:hover,
.pagination > .active > a:focus,
.pagination > .active > span:focus {
  z-index: 3;
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
  cursor: default;
}
.pagination > .disabled > span,
.pagination > .disabled > span:hover,
.pagination > .disabled > span:focus,
.pagination > .disabled > a,
.pagination > .disabled > a:hover,
.pagination > .disabled > a:focus {
  color: #777777;
  background-color: #fff;
  border-color: #ddd;
  cursor: not-allowed;
}
.pagination-lg > li > a,
.pagination-lg > li > span {
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
}
.pagination-lg > li:first-child > a,
.pagination-lg > li:first-child > span {
  border-bottom-left-radius: 3px;
  border-top-left-radius: 3px;
}
.pagination-lg > li:last-child > a,
.pagination-lg > li:last-child > span {
  border-bottom-right-radius: 3px;
  border-top-right-radius: 3px;
}
.pagination-sm > li > a,
.pagination-sm > li > span {
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
}
.pagination-sm > li:first-child > a,
.pagination-sm > li:first-child > span {
  border-bottom-left-radius: 1px;
  border-top-left-radius: 1px;
}
.pagination-sm > li:last-child > a,
.pagination-sm > li:last-child > span {
  border-bottom-right-radius: 1px;
  border-top-right-radius: 1px;
}
.pager {
  padding-left: 0;
  margin: 18px 0;
  list-style: none;
  text-align: center;
}
.pager li {
  display: inline;
}
.pager li > a,
.pager li > span {
  display: inline-block;
  padding: 5px 14px;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 15px;
}
.pager li > a:hover,
.pager li > a:focus {
  text-decoration: none;
  background-color: #eeeeee;
}
.pager .next > a,
.pager .next > span {
  float: right;
}
.pager .previous > a,
.pager .previous > span {
  float: left;
}
.pager .disabled > a,
.pager .disabled > a:hover,
.pager .disabled > a:focus,
.pager .disabled > span {
  color: #777777;
  background-color: #fff;
  cursor: not-allowed;
}
.label {
  display: inline;
  padding: .2em .6em .3em;
  font-size: 75%;
  font-weight: bold;
  line-height: 1;
  color: #fff;
  text-align: center;
  white-space: nowrap;
  vertical-align: baseline;
  border-radius: .25em;
}
a.label:hover,
a.label:focus {
  color: #fff;
  text-decoration: none;
  cursor: pointer;
}
.label:empty {
  display: none;
}
.btn .label {
  position: relative;
  top: -1px;
}
.label-default {
  background-color: #777777;
}
.label-default[href]:hover,
.label-default[href]:focus {
  background-color: #5e5e5e;
}
.label-primary {
  background-color: #337ab7;
}
.label-primary[href]:hover,
.label-primary[href]:focus {
  background-color: #286090;
}
.label-success {
  background-color: #5cb85c;
}
.label-success[href]:hover,
.label-success[href]:focus {
  background-color: #449d44;
}
.label-info {
  background-color: #5bc0de;
}
.label-info[href]:hover,
.label-info[href]:focus {
  background-color: #31b0d5;
}
.label-warning {
  background-color: #f0ad4e;
}
.label-warning[href]:hover,
.label-warning[href]:focus {
  background-color: #ec971f;
}
.label-danger {
  background-color: #d9534f;
}
.label-danger[href]:hover,
.label-danger[href]:focus {
  background-color: #c9302c;
}
.badge {
  display: inline-block;
  min-width: 10px;
  padding: 3px 7px;
  font-size: 12px;
  font-weight: bold;
  color: #fff;
  line-height: 1;
  vertical-align: middle;
  white-space: nowrap;
  text-align: center;
  background-color: #777777;
  border-radius: 10px;
}
.badge:empty {
  display: none;
}
.btn .badge {
  position: relative;
  top: -1px;
}
.btn-xs .badge,
.btn-group-xs > .btn .badge {
  top: 0;
  padding: 1px 5px;
}
a.badge:hover,
a.badge:focus {
  color: #fff;
  text-decoration: none;
  cursor: pointer;
}
.list-group-item.active > .badge,
.nav-pills > .active > a > .badge {
  color: #337ab7;
  background-color: #fff;
}
.list-group-item > .badge {
  float: right;
}
.list-group-item > .badge + .badge {
  margin-right: 5px;
}
.nav-pills > li > a > .badge {
  margin-left: 3px;
}
.jumbotron {
  padding-top: 30px;
  padding-bottom: 30px;
  margin-bottom: 30px;
  color: inherit;
  background-color: #eeeeee;
}
.jumbotron h1,
.jumbotron .h1 {
  color: inherit;
}
.jumbotron p {
  margin-bottom: 15px;
  font-size: 20px;
  font-weight: 200;
}
.jumbotron > hr {
  border-top-color: #d5d5d5;
}
.container .jumbotron,
.container-fluid .jumbotron {
  border-radius: 3px;
  padding-left: 0px;
  padding-right: 0px;
}
.jumbotron .container {
  max-width: 100%;
}
@media screen and (min-width: 768px) {
  .jumbotron {
    padding-top: 48px;
    padding-bottom: 48px;
  }
  .container .jumbotron,
  .container-fluid .jumbotron {
    padding-left: 60px;
    padding-right: 60px;
  }
  .jumbotron h1,
  .jumbotron .h1 {
    font-size: 59px;
  }
}
.thumbnail {
  display: block;
  padding: 4px;
  margin-bottom: 18px;
  line-height: 1.42857143;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 2px;
  -webkit-transition: border 0.2s ease-in-out;
  -o-transition: border 0.2s ease-in-out;
  transition: border 0.2s ease-in-out;
}
.thumbnail > img,
.thumbnail a > img {
  margin-left: auto;
  margin-right: auto;
}
a.thumbnail:hover,
a.thumbnail:focus,
a.thumbnail.active {
  border-color: #337ab7;
}
.thumbnail .caption {
  padding: 9px;
  color: #000;
}
.alert {
  padding: 15px;
  margin-bottom: 18px;
  border: 1px solid transparent;
  border-radius: 2px;
}
.alert h4 {
  margin-top: 0;
  color: inherit;
}
.alert .alert-link {
  font-weight: bold;
}
.alert > p,
.alert > ul {
  margin-bottom: 0;
}
.alert > p + p {
  margin-top: 5px;
}
.alert-dismissable,
.alert-dismissible {
  padding-right: 35px;
}
.alert-dismissable .close,
.alert-dismissible .close {
  position: relative;
  top: -2px;
  right: -21px;
  color: inherit;
}
.alert-success {
  background-color: #dff0d8;
  border-color: #d6e9c6;
  color: #3c763d;
}
.alert-success hr {
  border-top-color: #c9e2b3;
}
.alert-success .alert-link {
  color: #2b542c;
}
.alert-info {
  background-color: #d9edf7;
  border-color: #bce8f1;
  color: #31708f;
}
.alert-info hr {
  border-top-color: #a6e1ec;
}
.alert-info .alert-link {
  color: #245269;
}
.alert-warning {
  background-color: #fcf8e3;
  border-color: #faebcc;
  color: #8a6d3b;
}
.alert-warning hr {
  border-top-color: #f7e1b5;
}
.alert-warning .alert-link {
  color: #66512c;
}
.alert-danger {
  background-color: #f2dede;
  border-color: #ebccd1;
  color: #a94442;
}
.alert-danger hr {
  border-top-color: #e4b9c0;
}
.alert-danger .alert-link {
  color: #843534;
}
@-webkit-keyframes progress-bar-stripes {
  from {
    background-position: 40px 0;
  }
  to {
    background-position: 0 0;
  }
}
@keyframes progress-bar-stripes {
  from {
    background-position: 40px 0;
  }
  to {
    background-position: 0 0;
  }
}
.progress {
  overflow: hidden;
  height: 18px;
  margin-bottom: 18px;
  background-color: #f5f5f5;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
  box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
}
.progress-bar {
  float: left;
  width: 0%;
  height: 100%;
  font-size: 12px;
  line-height: 18px;
  color: #fff;
  text-align: center;
  background-color: #337ab7;
  -webkit-box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.15);
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.15);
  -webkit-transition: width 0.6s ease;
  -o-transition: width 0.6s ease;
  transition: width 0.6s ease;
}
.progress-striped .progress-bar,
.progress-bar-striped {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-size: 40px 40px;
}
.progress.active .progress-bar,
.progress-bar.active {
  -webkit-animation: progress-bar-stripes 2s linear infinite;
  -o-animation: progress-bar-stripes 2s linear infinite;
  animation: progress-bar-stripes 2s linear infinite;
}
.progress-bar-success {
  background-color: #5cb85c;
}
.progress-striped .progress-bar-success {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-info {
  background-color: #5bc0de;
}
.progress-striped .progress-bar-info {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-warning {
  background-color: #f0ad4e;
}
.progress-striped .progress-bar-warning {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-danger {
  background-color: #d9534f;
}
.progress-striped .progress-bar-danger {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.media {
  margin-top: 15px;
}
.media:first-child {
  margin-top: 0;
}
.media,
.media-body {
  zoom: 1;
  overflow: hidden;
}
.media-body {
  width: 10000px;
}
.media-object {
  display: block;
}
.media-object.img-thumbnail {
  max-width: none;
}
.media-right,
.media > .pull-right {
  padding-left: 10px;
}
.media-left,
.media > .pull-left {
  padding-right: 10px;
}
.media-left,
.media-right,
.media-body {
  display: table-cell;
  vertical-align: top;
}
.media-middle {
  vertical-align: middle;
}
.media-bottom {
  vertical-align: bottom;
}
.media-heading {
  margin-top: 0;
  margin-bottom: 5px;
}
.media-list {
  padding-left: 0;
  list-style: none;
}
.list-group {
  margin-bottom: 20px;
  padding-left: 0;
}
.list-group-item {
  position: relative;
  display: block;
  padding: 10px 15px;
  margin-bottom: -1px;
  background-color: #fff;
  border: 1px solid #ddd;
}
.list-group-item:first-child {
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
}
.list-group-item:last-child {
  margin-bottom: 0;
  border-bottom-right-radius: 2px;
  border-bottom-left-radius: 2px;
}
a.list-group-item,
button.list-group-item {
  color: #555;
}
a.list-group-item .list-group-item-heading,
button.list-group-item .list-group-item-heading {
  color: #333;
}
a.list-group-item:hover,
button.list-group-item:hover,
a.list-group-item:focus,
button.list-group-item:focus {
  text-decoration: none;
  color: #555;
  background-color: #f5f5f5;
}
button.list-group-item {
  width: 100%;
  text-align: left;
}
.list-group-item.disabled,
.list-group-item.disabled:hover,
.list-group-item.disabled:focus {
  background-color: #eeeeee;
  color: #777777;
  cursor: not-allowed;
}
.list-group-item.disabled .list-group-item-heading,
.list-group-item.disabled:hover .list-group-item-heading,
.list-group-item.disabled:focus .list-group-item-heading {
  color: inherit;
}
.list-group-item.disabled .list-group-item-text,
.list-group-item.disabled:hover .list-group-item-text,
.list-group-item.disabled:focus .list-group-item-text {
  color: #777777;
}
.list-group-item.active,
.list-group-item.active:hover,
.list-group-item.active:focus {
  z-index: 2;
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
}
.list-group-item.active .list-group-item-heading,
.list-group-item.active:hover .list-group-item-heading,
.list-group-item.active:focus .list-group-item-heading,
.list-group-item.active .list-group-item-heading > small,
.list-group-item.active:hover .list-group-item-heading > small,
.list-group-item.active:focus .list-group-item-heading > small,
.list-group-item.active .list-group-item-heading > .small,
.list-group-item.active:hover .list-group-item-heading > .small,
.list-group-item.active:focus .list-group-item-heading > .small {
  color: inherit;
}
.list-group-item.active .list-group-item-text,
.list-group-item.active:hover .list-group-item-text,
.list-group-item.active:focus .list-group-item-text {
  color: #c7ddef;
}
.list-group-item-success {
  color: #3c763d;
  background-color: #dff0d8;
}
a.list-group-item-success,
button.list-group-item-success {
  color: #3c763d;
}
a.list-group-item-success .list-group-item-heading,
button.list-group-item-success .list-group-item-heading {
  color: inherit;
}
a.list-group-item-success:hover,
button.list-group-item-success:hover,
a.list-group-item-success:focus,
button.list-group-item-success:focus {
  color: #3c763d;
  background-color: #d0e9c6;
}
a.list-group-item-success.active,
button.list-group-item-success.active,
a.list-group-item-success.active:hover,
button.list-group-item-success.active:hover,
a.list-group-item-success.active:focus,
button.list-group-item-success.active:focus {
  color: #fff;
  background-color: #3c763d;
  border-color: #3c763d;
}
.list-group-item-info {
  color: #31708f;
  background-color: #d9edf7;
}
a.list-group-item-info,
button.list-group-item-info {
  color: #31708f;
}
a.list-group-item-info .list-group-item-heading,
button.list-group-item-info .list-group-item-heading {
  color: inherit;
}
a.list-group-item-info:hover,
button.list-group-item-info:hover,
a.list-group-item-info:focus,
button.list-group-item-info:focus {
  color: #31708f;
  background-color: #c4e3f3;
}
a.list-group-item-info.active,
button.list-group-item-info.active,
a.list-group-item-info.active:hover,
button.list-group-item-info.active:hover,
a.list-group-item-info.active:focus,
button.list-group-item-info.active:focus {
  color: #fff;
  background-color: #31708f;
  border-color: #31708f;
}
.list-group-item-warning {
  color: #8a6d3b;
  background-color: #fcf8e3;
}
a.list-group-item-warning,
button.list-group-item-warning {
  color: #8a6d3b;
}
a.list-group-item-warning .list-group-item-heading,
button.list-group-item-warning .list-group-item-heading {
  color: inherit;
}
a.list-group-item-warning:hover,
button.list-group-item-warning:hover,
a.list-group-item-warning:focus,
button.list-group-item-warning:focus {
  color: #8a6d3b;
  background-color: #faf2cc;
}
a.list-group-item-warning.active,
button.list-group-item-warning.active,
a.list-group-item-warning.active:hover,
button.list-group-item-warning.active:hover,
a.list-group-item-warning.active:focus,
button.list-group-item-warning.active:focus {
  color: #fff;
  background-color: #8a6d3b;
  border-color: #8a6d3b;
}
.list-group-item-danger {
  color: #a94442;
  background-color: #f2dede;
}
a.list-group-item-danger,
button.list-group-item-danger {
  color: #a94442;
}
a.list-group-item-danger .list-group-item-heading,
button.list-group-item-danger .list-group-item-heading {
  color: inherit;
}
a.list-group-item-danger:hover,
button.list-group-item-danger:hover,
a.list-group-item-danger:focus,
button.list-group-item-danger:focus {
  color: #a94442;
  background-color: #ebcccc;
}
a.list-group-item-danger.active,
button.list-group-item-danger.active,
a.list-group-item-danger.active:hover,
button.list-group-item-danger.active:hover,
a.list-group-item-danger.active:focus,
button.list-group-item-danger.active:focus {
  color: #fff;
  background-color: #a94442;
  border-color: #a94442;
}
.list-group-item-heading {
  margin-top: 0;
  margin-bottom: 5px;
}
.list-group-item-text {
  margin-bottom: 0;
  line-height: 1.3;
}
.panel {
  margin-bottom: 18px;
  background-color: #fff;
  border: 1px solid transparent;
  border-radius: 2px;
  -webkit-box-shadow: 0 1px 1px rgba(0, 0, 0, 0.05);
  box-shadow: 0 1px 1px rgba(0, 0, 0, 0.05);
}
.panel-body {
  padding: 15px;
}
.panel-heading {
  padding: 10px 15px;
  border-bottom: 1px solid transparent;
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel-heading > .dropdown .dropdown-toggle {
  color: inherit;
}
.panel-title {
  margin-top: 0;
  margin-bottom: 0;
  font-size: 15px;
  color: inherit;
}
.panel-title > a,
.panel-title > small,
.panel-title > .small,
.panel-title > small > a,
.panel-title > .small > a {
  color: inherit;
}
.panel-footer {
  padding: 10px 15px;
  background-color: #f5f5f5;
  border-top: 1px solid #ddd;
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .list-group,
.panel > .panel-collapse > .list-group {
  margin-bottom: 0;
}
.panel > .list-group .list-group-item,
.panel > .panel-collapse > .list-group .list-group-item {
  border-width: 1px 0;
  border-radius: 0;
}
.panel > .list-group:first-child .list-group-item:first-child,
.panel > .panel-collapse > .list-group:first-child .list-group-item:first-child {
  border-top: 0;
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel > .list-group:last-child .list-group-item:last-child,
.panel > .panel-collapse > .list-group:last-child .list-group-item:last-child {
  border-bottom: 0;
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .panel-heading + .panel-collapse > .list-group .list-group-item:first-child {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.panel-heading + .list-group .list-group-item:first-child {
  border-top-width: 0;
}
.list-group + .panel-footer {
  border-top-width: 0;
}
.panel > .table,
.panel > .table-responsive > .table,
.panel > .panel-collapse > .table {
  margin-bottom: 0;
}
.panel > .table caption,
.panel > .table-responsive > .table caption,
.panel > .panel-collapse > .table caption {
  padding-left: 15px;
  padding-right: 15px;
}
.panel > .table:first-child,
.panel > .table-responsive:first-child > .table:first-child {
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child {
  border-top-left-radius: 1px;
  border-top-right-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child td:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child td:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child td:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child td:first-child,
.panel > .table:first-child > thead:first-child > tr:first-child th:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child th:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child th:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child th:first-child {
  border-top-left-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child td:last-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child td:last-child,
.panel > .table:first-child > tbody:first-child > tr:first-child td:last-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child td:last-child,
.panel > .table:first-child > thead:first-child > tr:first-child th:last-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child th:last-child,
.panel > .table:first-child > tbody:first-child > tr:first-child th:last-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child th:last-child {
  border-top-right-radius: 1px;
}
.panel > .table:last-child,
.panel > .table-responsive:last-child > .table:last-child {
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child {
  border-bottom-left-radius: 1px;
  border-bottom-right-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child td:first-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child td:first-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child td:first-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child td:first-child,
.panel > .table:last-child > tbody:last-child > tr:last-child th:first-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child th:first-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child th:first-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child th:first-child {
  border-bottom-left-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child td:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child td:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child td:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child td:last-child,
.panel > .table:last-child > tbody:last-child > tr:last-child th:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child th:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child th:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child th:last-child {
  border-bottom-right-radius: 1px;
}
.panel > .panel-body + .table,
.panel > .panel-body + .table-responsive,
.panel > .table + .panel-body,
.panel > .table-responsive + .panel-body {
  border-top: 1px solid #ddd;
}
.panel > .table > tbody:first-child > tr:first-child th,
.panel > .table > tbody:first-child > tr:first-child td {
  border-top: 0;
}
.panel > .table-bordered,
.panel > .table-responsive > .table-bordered {
  border: 0;
}
.panel > .table-bordered > thead > tr > th:first-child,
.panel > .table-responsive > .table-bordered > thead > tr > th:first-child,
.panel > .table-bordered > tbody > tr > th:first-child,
.panel > .table-responsive > .table-bordered > tbody > tr > th:first-child,
.panel > .table-bordered > tfoot > tr > th:first-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > th:first-child,
.panel > .table-bordered > thead > tr > td:first-child,
.panel > .table-responsive > .table-bordered > thead > tr > td:first-child,
.panel > .table-bordered > tbody > tr > td:first-child,
.panel > .table-responsive > .table-bordered > tbody > tr > td:first-child,
.panel > .table-bordered > tfoot > tr > td:first-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > td:first-child {
  border-left: 0;
}
.panel > .table-bordered > thead > tr > th:last-child,
.panel > .table-responsive > .table-bordered > thead > tr > th:last-child,
.panel > .table-bordered > tbody > tr > th:last-child,
.panel > .table-responsive > .table-bordered > tbody > tr > th:last-child,
.panel > .table-bordered > tfoot > tr > th:last-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > th:last-child,
.panel > .table-bordered > thead > tr > td:last-child,
.panel > .table-responsive > .table-bordered > thead > tr > td:last-child,
.panel > .table-bordered > tbody > tr > td:last-child,
.panel > .table-responsive > .table-bordered > tbody > tr > td:last-child,
.panel > .table-bordered > tfoot > tr > td:last-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > td:last-child {
  border-right: 0;
}
.panel > .table-bordered > thead > tr:first-child > td,
.panel > .table-responsive > .table-bordered > thead > tr:first-child > td,
.panel > .table-bordered > tbody > tr:first-child > td,
.panel > .table-responsive > .table-bordered > tbody > tr:first-child > td,
.panel > .table-bordered > thead > tr:first-child > th,
.panel > .table-responsive > .table-bordered > thead > tr:first-child > th,
.panel > .table-bordered > tbody > tr:first-child > th,
.panel > .table-responsive > .table-bordered > tbody > tr:first-child > th {
  border-bottom: 0;
}
.panel > .table-bordered > tbody > tr:last-child > td,
.panel > .table-responsive > .table-bordered > tbody > tr:last-child > td,
.panel > .table-bordered > tfoot > tr:last-child > td,
.panel > .table-responsive > .table-bordered > tfoot > tr:last-child > td,
.panel > .table-bordered > tbody > tr:last-child > th,
.panel > .table-responsive > .table-bordered > tbody > tr:last-child > th,
.panel > .table-bordered > tfoot > tr:last-child > th,
.panel > .table-responsive > .table-bordered > tfoot > tr:last-child > th {
  border-bottom: 0;
}
.panel > .table-responsive {
  border: 0;
  margin-bottom: 0;
}
.panel-group {
  margin-bottom: 18px;
}
.panel-group .panel {
  margin-bottom: 0;
  border-radius: 2px;
}
.panel-group .panel + .panel {
  margin-top: 5px;
}
.panel-group .panel-heading {
  border-bottom: 0;
}
.panel-group .panel-heading + .panel-collapse > .panel-body,
.panel-group .panel-heading + .panel-collapse > .list-group {
  border-top: 1px solid #ddd;
}
.panel-group .panel-footer {
  border-top: 0;
}
.panel-group .panel-footer + .panel-collapse .panel-body {
  border-bottom: 1px solid #ddd;
}
.panel-default {
  border-color: #ddd;
}
.panel-default > .panel-heading {
  color: #333333;
  background-color: #f5f5f5;
  border-color: #ddd;
}
.panel-default > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #ddd;
}
.panel-default > .panel-heading .badge {
  color: #f5f5f5;
  background-color: #333333;
}
.panel-default > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #ddd;
}
.panel-primary {
  border-color: #337ab7;
}
.panel-primary > .panel-heading {
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
}
.panel-primary > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #337ab7;
}
.panel-primary > .panel-heading .badge {
  color: #337ab7;
  background-color: #fff;
}
.panel-primary > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #337ab7;
}
.panel-success {
  border-color: #d6e9c6;
}
.panel-success > .panel-heading {
  color: #3c763d;
  background-color: #dff0d8;
  border-color: #d6e9c6;
}
.panel-success > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #d6e9c6;
}
.panel-success > .panel-heading .badge {
  color: #dff0d8;
  background-color: #3c763d;
}
.panel-success > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #d6e9c6;
}
.panel-info {
  border-color: #bce8f1;
}
.panel-info > .panel-heading {
  color: #31708f;
  background-color: #d9edf7;
  border-color: #bce8f1;
}
.panel-info > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #bce8f1;
}
.panel-info > .panel-heading .badge {
  color: #d9edf7;
  background-color: #31708f;
}
.panel-info > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #bce8f1;
}
.panel-warning {
  border-color: #faebcc;
}
.panel-warning > .panel-heading {
  color: #8a6d3b;
  background-color: #fcf8e3;
  border-color: #faebcc;
}
.panel-warning > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #faebcc;
}
.panel-warning > .panel-heading .badge {
  color: #fcf8e3;
  background-color: #8a6d3b;
}
.panel-warning > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #faebcc;
}
.panel-danger {
  border-color: #ebccd1;
}
.panel-danger > .panel-heading {
  color: #a94442;
  background-color: #f2dede;
  border-color: #ebccd1;
}
.panel-danger > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #ebccd1;
}
.panel-danger > .panel-heading .badge {
  color: #f2dede;
  background-color: #a94442;
}
.panel-danger > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #ebccd1;
}
.embed-responsive {
  position: relative;
  display: block;
  height: 0;
  padding: 0;
  overflow: hidden;
}
.embed-responsive .embed-responsive-item,
.embed-responsive iframe,
.embed-responsive embed,
.embed-responsive object,
.embed-responsive video {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  height: 100%;
  width: 100%;
  border: 0;
}
.embed-responsive-16by9 {
  padding-bottom: 56.25%;
}
.embed-responsive-4by3 {
  padding-bottom: 75%;
}
.well {
  min-height: 20px;
  padding: 19px;
  margin-bottom: 20px;
  background-color: #f5f5f5;
  border: 1px solid #e3e3e3;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05);
}
.well blockquote {
  border-color: #ddd;
  border-color: rgba(0, 0, 0, 0.15);
}
.well-lg {
  padding: 24px;
  border-radius: 3px;
}
.well-sm {
  padding: 9px;
  border-radius: 1px;
}
.close {
  float: right;
  font-size: 19.5px;
  font-weight: bold;
  line-height: 1;
  color: #000;
  text-shadow: 0 1px 0 #fff;
  opacity: 0.2;
  filter: alpha(opacity=20);
}
.close:hover,
.close:focus {
  color: #000;
  text-decoration: none;
  cursor: pointer;
  opacity: 0.5;
  filter: alpha(opacity=50);
}
button.close {
  padding: 0;
  cursor: pointer;
  background: transparent;
  border: 0;
  -webkit-appearance: none;
}
.modal-open {
  overflow: hidden;
}
.modal {
  display: none;
  overflow: hidden;
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 1050;
  -webkit-overflow-scrolling: touch;
  outline: 0;
}
.modal.fade .modal-dialog {
  -webkit-transform: translate(0, -25%);
  -ms-transform: translate(0, -25%);
  -o-transform: translate(0, -25%);
  transform: translate(0, -25%);
  -webkit-transition: -webkit-transform 0.3s ease-out;
  -moz-transition: -moz-transform 0.3s ease-out;
  -o-transition: -o-transform 0.3s ease-out;
  transition: transform 0.3s ease-out;
}
.modal.in .modal-dialog {
  -webkit-transform: translate(0, 0);
  -ms-transform: translate(0, 0);
  -o-transform: translate(0, 0);
  transform: translate(0, 0);
}
.modal-open .modal {
  overflow-x: hidden;
  overflow-y: auto;
}
.modal-dialog {
  position: relative;
  width: auto;
  margin: 10px;
}
.modal-content {
  position: relative;
  background-color: #fff;
  border: 1px solid #999;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-radius: 3px;
  -webkit-box-shadow: 0 3px 9px rgba(0, 0, 0, 0.5);
  box-shadow: 0 3px 9px rgba(0, 0, 0, 0.5);
  background-clip: padding-box;
  outline: 0;
}
.modal-backdrop {
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 1040;
  background-color: #000;
}
.modal-backdrop.fade {
  opacity: 0;
  filter: alpha(opacity=0);
}
.modal-backdrop.in {
  opacity: 0.5;
  filter: alpha(opacity=50);
}
.modal-header {
  padding: 15px;
  border-bottom: 1px solid #e5e5e5;
}
.modal-header .close {
  margin-top: -2px;
}
.modal-title {
  margin: 0;
  line-height: 1.42857143;
}
.modal-body {
  position: relative;
  padding: 15px;
}
.modal-footer {
  padding: 15px;
  text-align: right;
  border-top: 1px solid #e5e5e5;
}
.modal-footer .btn + .btn {
  margin-left: 5px;
  margin-bottom: 0;
}
.modal-footer .btn-group .btn + .btn {
  margin-left: -1px;
}
.modal-footer .btn-block + .btn-block {
  margin-left: 0;
}
.modal-scrollbar-measure {
  position: absolute;
  top: -9999px;
  width: 50px;
  height: 50px;
  overflow: scroll;
}
@media (min-width: 768px) {
  .modal-dialog {
    width: 600px;
    margin: 30px auto;
  }
  .modal-content {
    -webkit-box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
  }
  .modal-sm {
    width: 300px;
  }
}
@media (min-width: 992px) {
  .modal-lg {
    width: 900px;
  }
}
.tooltip {
  position: absolute;
  z-index: 1070;
  display: block;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  letter-spacing: normal;
  line-break: auto;
  line-height: 1.42857143;
  text-align: left;
  text-align: start;
  text-decoration: none;
  text-shadow: none;
  text-transform: none;
  white-space: normal;
  word-break: normal;
  word-spacing: normal;
  word-wrap: normal;
  font-size: 12px;
  opacity: 0;
  filter: alpha(opacity=0);
}
.tooltip.in {
  opacity: 0.9;
  filter: alpha(opacity=90);
}
.tooltip.top {
  margin-top: -3px;
  padding: 5px 0;
}
.tooltip.right {
  margin-left: 3px;
  padding: 0 5px;
}
.tooltip.bottom {
  margin-top: 3px;
  padding: 5px 0;
}
.tooltip.left {
  margin-left: -3px;
  padding: 0 5px;
}
.tooltip-inner {
  max-width: 200px;
  padding: 3px 8px;
  color: #fff;
  text-align: center;
  background-color: #000;
  border-radius: 2px;
}
.tooltip-arrow {
  position: absolute;
  width: 0;
  height: 0;
  border-color: transparent;
  border-style: solid;
}
.tooltip.top .tooltip-arrow {
  bottom: 0;
  left: 50%;
  margin-left: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.top-left .tooltip-arrow {
  bottom: 0;
  right: 5px;
  margin-bottom: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.top-right .tooltip-arrow {
  bottom: 0;
  left: 5px;
  margin-bottom: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.right .tooltip-arrow {
  top: 50%;
  left: 0;
  margin-top: -5px;
  border-width: 5px 5px 5px 0;
  border-right-color: #000;
}
.tooltip.left .tooltip-arrow {
  top: 50%;
  right: 0;
  margin-top: -5px;
  border-width: 5px 0 5px 5px;
  border-left-color: #000;
}
.tooltip.bottom .tooltip-arrow {
  top: 0;
  left: 50%;
  margin-left: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.tooltip.bottom-left .tooltip-arrow {
  top: 0;
  right: 5px;
  margin-top: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.tooltip.bottom-right .tooltip-arrow {
  top: 0;
  left: 5px;
  margin-top: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.popover {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 1060;
  display: none;
  max-width: 276px;
  padding: 1px;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  letter-spacing: normal;
  line-break: auto;
  line-height: 1.42857143;
  text-align: left;
  text-align: start;
  text-decoration: none;
  text-shadow: none;
  text-transform: none;
  white-space: normal;
  word-break: normal;
  word-spacing: normal;
  word-wrap: normal;
  font-size: 13px;
  background-color: #fff;
  background-clip: padding-box;
  border: 1px solid #ccc;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-radius: 3px;
  -webkit-box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
}
.popover.top {
  margin-top: -10px;
}
.popover.right {
  margin-left: 10px;
}
.popover.bottom {
  margin-top: 10px;
}
.popover.left {
  margin-left: -10px;
}
.popover-title {
  margin: 0;
  padding: 8px 14px;
  font-size: 13px;
  background-color: #f7f7f7;
  border-bottom: 1px solid #ebebeb;
  border-radius: 2px 2px 0 0;
}
.popover-content {
  padding: 9px 14px;
}
.popover > .arrow,
.popover > .arrow:after {
  position: absolute;
  display: block;
  width: 0;
  height: 0;
  border-color: transparent;
  border-style: solid;
}
.popover > .arrow {
  border-width: 11px;
}
.popover > .arrow:after {
  border-width: 10px;
  content: "";
}
.popover.top > .arrow {
  left: 50%;
  margin-left: -11px;
  border-bottom-width: 0;
  border-top-color: #999999;
  border-top-color: rgba(0, 0, 0, 0.25);
  bottom: -11px;
}
.popover.top > .arrow:after {
  content: " ";
  bottom: 1px;
  margin-left: -10px;
  border-bottom-width: 0;
  border-top-color: #fff;
}
.popover.right > .arrow {
  top: 50%;
  left: -11px;
  margin-top: -11px;
  border-left-width: 0;
  border-right-color: #999999;
  border-right-color: rgba(0, 0, 0, 0.25);
}
.popover.right > .arrow:after {
  content: " ";
  left: 1px;
  bottom: -10px;
  border-left-width: 0;
  border-right-color: #fff;
}
.popover.bottom > .arrow {
  left: 50%;
  margin-left: -11px;
  border-top-width: 0;
  border-bottom-color: #999999;
  border-bottom-color: rgba(0, 0, 0, 0.25);
  top: -11px;
}
.popover.bottom > .arrow:after {
  content: " ";
  top: 1px;
  margin-left: -10px;
  border-top-width: 0;
  border-bottom-color: #fff;
}
.popover.left > .arrow {
  top: 50%;
  right: -11px;
  margin-top: -11px;
  border-right-width: 0;
  border-left-color: #999999;
  border-left-color: rgba(0, 0, 0, 0.25);
}
.popover.left > .arrow:after {
  content: " ";
  right: 1px;
  border-right-width: 0;
  border-left-color: #fff;
  bottom: -10px;
}
.carousel {
  position: relative;
}
.carousel-inner {
  position: relative;
  overflow: hidden;
  width: 100%;
}
.carousel-inner > .item {
  display: none;
  position: relative;
  -webkit-transition: 0.6s ease-in-out left;
  -o-transition: 0.6s ease-in-out left;
  transition: 0.6s ease-in-out left;
}
.carousel-inner > .item > img,
.carousel-inner > .item > a > img {
  line-height: 1;
}
@media all and (transform-3d), (-webkit-transform-3d) {
  .carousel-inner > .item {
    -webkit-transition: -webkit-transform 0.6s ease-in-out;
    -moz-transition: -moz-transform 0.6s ease-in-out;
    -o-transition: -o-transform 0.6s ease-in-out;
    transition: transform 0.6s ease-in-out;
    -webkit-backface-visibility: hidden;
    -moz-backface-visibility: hidden;
    backface-visibility: hidden;
    -webkit-perspective: 1000px;
    -moz-perspective: 1000px;
    perspective: 1000px;
  }
  .carousel-inner > .item.next,
  .carousel-inner > .item.active.right {
    -webkit-transform: translate3d(100%, 0, 0);
    transform: translate3d(100%, 0, 0);
    left: 0;
  }
  .carousel-inner > .item.prev,
  .carousel-inner > .item.active.left {
    -webkit-transform: translate3d(-100%, 0, 0);
    transform: translate3d(-100%, 0, 0);
    left: 0;
  }
  .carousel-inner > .item.next.left,
  .carousel-inner > .item.prev.right,
  .carousel-inner > .item.active {
    -webkit-transform: translate3d(0, 0, 0);
    transform: translate3d(0, 0, 0);
    left: 0;
  }
}
.carousel-inner > .active,
.carousel-inner > .next,
.carousel-inner > .prev {
  display: block;
}
.carousel-inner > .active {
  left: 0;
}
.carousel-inner > .next,
.carousel-inner > .prev {
  position: absolute;
  top: 0;
  width: 100%;
}
.carousel-inner > .next {
  left: 100%;
}
.carousel-inner > .prev {
  left: -100%;
}
.carousel-inner > .next.left,
.carousel-inner > .prev.right {
  left: 0;
}
.carousel-inner > .active.left {
  left: -100%;
}
.carousel-inner > .active.right {
  left: 100%;
}
.carousel-control {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  width: 15%;
  opacity: 0.5;
  filter: alpha(opacity=50);
  font-size: 20px;
  color: #fff;
  text-align: center;
  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.6);
  background-color: rgba(0, 0, 0, 0);
}
.carousel-control.left {
  background-image: -webkit-linear-gradient(left, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-image: -o-linear-gradient(left, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-repeat: repeat-x;
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#80000000', endColorstr='#00000000', GradientType=1);
}
.carousel-control.right {
  left: auto;
  right: 0;
  background-image: -webkit-linear-gradient(left, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-image: -o-linear-gradient(left, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-repeat: repeat-x;
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#00000000', endColorstr='#80000000', GradientType=1);
}
.carousel-control:hover,
.carousel-control:focus {
  outline: 0;
  color: #fff;
  text-decoration: none;
  opacity: 0.9;
  filter: alpha(opacity=90);
}
.carousel-control .icon-prev,
.carousel-control .icon-next,
.carousel-control .glyphicon-chevron-left,
.carousel-control .glyphicon-chevron-right {
  position: absolute;
  top: 50%;
  margin-top: -10px;
  z-index: 5;
  display: inline-block;
}
.carousel-control .icon-prev,
.carousel-control .glyphicon-chevron-left {
  left: 50%;
  margin-left: -10px;
}
.carousel-control .icon-next,
.carousel-control .glyphicon-chevron-right {
  right: 50%;
  margin-right: -10px;
}
.carousel-control .icon-prev,
.carousel-control .icon-next {
  width: 20px;
  height: 20px;
  line-height: 1;
  font-family: serif;
}
.carousel-control .icon-prev:before {
  content: '\2039';
}
.carousel-control .icon-next:before {
  content: '\203a';
}
.carousel-indicators {
  position: absolute;
  bottom: 10px;
  left: 50%;
  z-index: 15;
  width: 60%;
  margin-left: -30%;
  padding-left: 0;
  list-style: none;
  text-align: center;
}
.carousel-indicators li {
  display: inline-block;
  width: 10px;
  height: 10px;
  margin: 1px;
  text-indent: -999px;
  border: 1px solid #fff;
  border-radius: 10px;
  cursor: pointer;
  background-color: #000 \9;
  background-color: rgba(0, 0, 0, 0);
}
.carousel-indicators .active {
  margin: 0;
  width: 12px;
  height: 12px;
  background-color: #fff;
}
.carousel-caption {
  position: absolute;
  left: 15%;
  right: 15%;
  bottom: 20px;
  z-index: 10;
  padding-top: 20px;
  padding-bottom: 20px;
  color: #fff;
  text-align: center;
  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.6);
}
.carousel-caption .btn {
  text-shadow: none;
}
@media screen and (min-width: 768px) {
  .carousel-control .glyphicon-chevron-left,
  .carousel-control .glyphicon-chevron-right,
  .carousel-control .icon-prev,
  .carousel-control .icon-next {
    width: 30px;
    height: 30px;
    margin-top: -10px;
    font-size: 30px;
  }
  .carousel-control .glyphicon-chevron-left,
  .carousel-control .icon-prev {
    margin-left: -10px;
  }
  .carousel-control .glyphicon-chevron-right,
  .carousel-control .icon-next {
    margin-right: -10px;
  }
  .carousel-caption {
    left: 20%;
    right: 20%;
    padding-bottom: 30px;
  }
  .carousel-indicators {
    bottom: 20px;
  }
}
.clearfix:before,
.clearfix:after,
.dl-horizontal dd:before,
.dl-horizontal dd:after,
.container:before,
.container:after,
.container-fluid:before,
.container-fluid:after,
.row:before,
.row:after,
.form-horizontal .form-group:before,
.form-horizontal .form-group:after,
.btn-toolbar:before,
.btn-toolbar:after,
.btn-group-vertical > .btn-group:before,
.btn-group-vertical > .btn-group:after,
.nav:before,
.nav:after,
.navbar:before,
.navbar:after,
.navbar-header:before,
.navbar-header:after,
.navbar-collapse:before,
.navbar-collapse:after,
.pager:before,
.pager:after,
.panel-body:before,
.panel-body:after,
.modal-header:before,
.modal-header:after,
.modal-footer:before,
.modal-footer:after,
.item_buttons:before,
.item_buttons:after {
  content: " ";
  display: table;
}
.clearfix:after,
.dl-horizontal dd:after,
.container:after,
.container-fluid:after,
.row:after,
.form-horizontal .form-group:after,
.btn-toolbar:after,
.btn-group-vertical > .btn-group:after,
.nav:after,
.navbar:after,
.navbar-header:after,
.navbar-collapse:after,
.pager:after,
.panel-body:after,
.modal-header:after,
.modal-footer:after,
.item_buttons:after {
  clear: both;
}
.center-block {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.pull-right {
  float: right !important;
}
.pull-left {
  float: left !important;
}
.hide {
  display: none !important;
}
.show {
  display: block !important;
}
.invisible {
  visibility: hidden;
}
.text-hide {
  font: 0/0 a;
  color: transparent;
  text-shadow: none;
  background-color: transparent;
  border: 0;
}
.hidden {
  display: none !important;
}
.affix {
  position: fixed;
}
@-ms-viewport {
  width: device-width;
}
.visible-xs,
.visible-sm,
.visible-md,
.visible-lg {
  display: none !important;
}
.visible-xs-block,
.visible-xs-inline,
.visible-xs-inline-block,
.visible-sm-block,
.visible-sm-inline,
.visible-sm-inline-block,
.visible-md-block,
.visible-md-inline,
.visible-md-inline-block,
.visible-lg-block,
.visible-lg-inline,
.visible-lg-inline-block {
  display: none !important;
}
@media (max-width: 767px) {
  .visible-xs {
    display: block !important;
  }
  table.visible-xs {
    display: table !important;
  }
  tr.visible-xs {
    display: table-row !important;
  }
  th.visible-xs,
  td.visible-xs {
    display: table-cell !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-block {
    display: block !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-inline {
    display: inline !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm {
    display: block !important;
  }
  table.visible-sm {
    display: table !important;
  }
  tr.visible-sm {
    display: table-row !important;
  }
  th.visible-sm,
  td.visible-sm {
    display: table-cell !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-block {
    display: block !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-inline {
    display: inline !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md {
    display: block !important;
  }
  table.visible-md {
    display: table !important;
  }
  tr.visible-md {
    display: table-row !important;
  }
  th.visible-md,
  td.visible-md {
    display: table-cell !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-block {
    display: block !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-inline {
    display: inline !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg {
    display: block !important;
  }
  table.visible-lg {
    display: table !important;
  }
  tr.visible-lg {
    display: table-row !important;
  }
  th.visible-lg,
  td.visible-lg {
    display: table-cell !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-block {
    display: block !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-inline {
    display: inline !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-inline-block {
    display: inline-block !important;
  }
}
@media (max-width: 767px) {
  .hidden-xs {
    display: none !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .hidden-sm {
    display: none !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .hidden-md {
    display: none !important;
  }
}
@media (min-width: 1200px) {
  .hidden-lg {
    display: none !important;
  }
}
.visible-print {
  display: none !important;
}
@media print {
  .visible-print {
    display: block !important;
  }
  table.visible-print {
    display: table !important;
  }
  tr.visible-print {
    display: table-row !important;
  }
  th.visible-print,
  td.visible-print {
    display: table-cell !important;
  }
}
.visible-print-block {
  display: none !important;
}
@media print {
  .visible-print-block {
    display: block !important;
  }
}
.visible-print-inline {
  display: none !important;
}
@media print {
  .visible-print-inline {
    display: inline !important;
  }
}
.visible-print-inline-block {
  display: none !important;
}
@media print {
  .visible-print-inline-block {
    display: inline-block !important;
  }
}
@media print {
  .hidden-print {
    display: none !important;
  }
}
/*!
*
* Font Awesome
*
*/
/*!
 *  Font Awesome 4.2.0 by @davegandy - http://fontawesome.io - @fontawesome
 *  License - http://fontawesome.io/license (Font: SIL OFL 1.1, CSS: MIT License)
 */
/* FONT PATH
 * -------------------------- */
@font-face {
  font-family: 'FontAwesome';
  src: url('../components/font-awesome/fonts/fontawesome-webfont.eot?v=4.2.0');
  src: url('../components/font-awesome/fonts/fontawesome-webfont.eot?#iefix&v=4.2.0') format('embedded-opentype'), url('../components/font-awesome/fonts/fontawesome-webfont.woff?v=4.2.0') format('woff'), url('../components/font-awesome/fonts/fontawesome-webfont.ttf?v=4.2.0') format('truetype'), url('../components/font-awesome/fonts/fontawesome-webfont.svg?v=4.2.0#fontawesomeregular') format('svg');
  font-weight: normal;
  font-style: normal;
}
.fa {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
/* makes the font 33% larger relative to the icon container */
.fa-lg {
  font-size: 1.33333333em;
  line-height: 0.75em;
  vertical-align: -15%;
}
.fa-2x {
  font-size: 2em;
}
.fa-3x {
  font-size: 3em;
}
.fa-4x {
  font-size: 4em;
}
.fa-5x {
  font-size: 5em;
}
.fa-fw {
  width: 1.28571429em;
  text-align: center;
}
.fa-ul {
  padding-left: 0;
  margin-left: 2.14285714em;
  list-style-type: none;
}
.fa-ul > li {
  position: relative;
}
.fa-li {
  position: absolute;
  left: -2.14285714em;
  width: 2.14285714em;
  top: 0.14285714em;
  text-align: center;
}
.fa-li.fa-lg {
  left: -1.85714286em;
}
.fa-border {
  padding: .2em .25em .15em;
  border: solid 0.08em #eee;
  border-radius: .1em;
}
.pull-right {
  float: right;
}
.pull-left {
  float: left;
}
.fa.pull-left {
  margin-right: .3em;
}
.fa.pull-right {
  margin-left: .3em;
}
.fa-spin {
  -webkit-animation: fa-spin 2s infinite linear;
  animation: fa-spin 2s infinite linear;
}
@-webkit-keyframes fa-spin {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(359deg);
    transform: rotate(359deg);
  }
}
@keyframes fa-spin {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(359deg);
    transform: rotate(359deg);
  }
}
.fa-rotate-90 {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=1);
  -webkit-transform: rotate(90deg);
  -ms-transform: rotate(90deg);
  transform: rotate(90deg);
}
.fa-rotate-180 {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=2);
  -webkit-transform: rotate(180deg);
  -ms-transform: rotate(180deg);
  transform: rotate(180deg);
}
.fa-rotate-270 {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=3);
  -webkit-transform: rotate(270deg);
  -ms-transform: rotate(270deg);
  transform: rotate(270deg);
}
.fa-flip-horizontal {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=0, mirror=1);
  -webkit-transform: scale(-1, 1);
  -ms-transform: scale(-1, 1);
  transform: scale(-1, 1);
}
.fa-flip-vertical {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=2, mirror=1);
  -webkit-transform: scale(1, -1);
  -ms-transform: scale(1, -1);
  transform: scale(1, -1);
}
:root .fa-rotate-90,
:root .fa-rotate-180,
:root .fa-rotate-270,
:root .fa-flip-horizontal,
:root .fa-flip-vertical {
  filter: none;
}
.fa-stack {
  position: relative;
  display: inline-block;
  width: 2em;
  height: 2em;
  line-height: 2em;
  vertical-align: middle;
}
.fa-stack-1x,
.fa-stack-2x {
  position: absolute;
  left: 0;
  width: 100%;
  text-align: center;
}
.fa-stack-1x {
  line-height: inherit;
}
.fa-stack-2x {
  font-size: 2em;
}
.fa-inverse {
  color: #fff;
}
/* Font Awesome uses the Unicode Private Use Area (PUA) to ensure screen
   readers do not read off random characters that represent icons */
.fa-glass:before {
  content: "\f000";
}
.fa-music:before {
  content: "\f001";
}
.fa-search:before {
  content: "\f002";
}
.fa-envelope-o:before {
  content: "\f003";
}
.fa-heart:before {
  content: "\f004";
}
.fa-star:before {
  content: "\f005";
}
.fa-star-o:before {
  content: "\f006";
}
.fa-user:before {
  content: "\f007";
}
.fa-film:before {
  content: "\f008";
}
.fa-th-large:before {
  content: "\f009";
}
.fa-th:before {
  content: "\f00a";
}
.fa-th-list:before {
  content: "\f00b";
}
.fa-check:before {
  content: "\f00c";
}
.fa-remove:before,
.fa-close:before,
.fa-times:before {
  content: "\f00d";
}
.fa-search-plus:before {
  content: "\f00e";
}
.fa-search-minus:before {
  content: "\f010";
}
.fa-power-off:before {
  content: "\f011";
}
.fa-signal:before {
  content: "\f012";
}
.fa-gear:before,
.fa-cog:before {
  content: "\f013";
}
.fa-trash-o:before {
  content: "\f014";
}
.fa-home:before {
  content: "\f015";
}
.fa-file-o:before {
  content: "\f016";
}
.fa-clock-o:before {
  content: "\f017";
}
.fa-road:before {
  content: "\f018";
}
.fa-download:before {
  content: "\f019";
}
.fa-arrow-circle-o-down:before {
  content: "\f01a";
}
.fa-arrow-circle-o-up:before {
  content: "\f01b";
}
.fa-inbox:before {
  content: "\f01c";
}
.fa-play-circle-o:before {
  content: "\f01d";
}
.fa-rotate-right:before,
.fa-repeat:before {
  content: "\f01e";
}
.fa-refresh:before {
  content: "\f021";
}
.fa-list-alt:before {
  content: "\f022";
}
.fa-lock:before {
  content: "\f023";
}
.fa-flag:before {
  content: "\f024";
}
.fa-headphones:before {
  content: "\f025";
}
.fa-volume-off:before {
  content: "\f026";
}
.fa-volume-down:before {
  content: "\f027";
}
.fa-volume-up:before {
  content: "\f028";
}
.fa-qrcode:before {
  content: "\f029";
}
.fa-barcode:before {
  content: "\f02a";
}
.fa-tag:before {
  content: "\f02b";
}
.fa-tags:before {
  content: "\f02c";
}
.fa-book:before {
  content: "\f02d";
}
.fa-bookmark:before {
  content: "\f02e";
}
.fa-print:before {
  content: "\f02f";
}
.fa-camera:before {
  content: "\f030";
}
.fa-font:before {
  content: "\f031";
}
.fa-bold:before {
  content: "\f032";
}
.fa-italic:before {
  content: "\f033";
}
.fa-text-height:before {
  content: "\f034";
}
.fa-text-width:before {
  content: "\f035";
}
.fa-align-left:before {
  content: "\f036";
}
.fa-align-center:before {
  content: "\f037";
}
.fa-align-right:before {
  content: "\f038";
}
.fa-align-justify:before {
  content: "\f039";
}
.fa-list:before {
  content: "\f03a";
}
.fa-dedent:before,
.fa-outdent:before {
  content: "\f03b";
}
.fa-indent:before {
  content: "\f03c";
}
.fa-video-camera:before {
  content: "\f03d";
}
.fa-photo:before,
.fa-image:before,
.fa-picture-o:before {
  content: "\f03e";
}
.fa-pencil:before {
  content: "\f040";
}
.fa-map-marker:before {
  content: "\f041";
}
.fa-adjust:before {
  content: "\f042";
}
.fa-tint:before {
  content: "\f043";
}
.fa-edit:before,
.fa-pencil-square-o:before {
  content: "\f044";
}
.fa-share-square-o:before {
  content: "\f045";
}
.fa-check-square-o:before {
  content: "\f046";
}
.fa-arrows:before {
  content: "\f047";
}
.fa-step-backward:before {
  content: "\f048";
}
.fa-fast-backward:before {
  content: "\f049";
}
.fa-backward:before {
  content: "\f04a";
}
.fa-play:before {
  content: "\f04b";
}
.fa-pause:before {
  content: "\f04c";
}
.fa-stop:before {
  content: "\f04d";
}
.fa-forward:before {
  content: "\f04e";
}
.fa-fast-forward:before {
  content: "\f050";
}
.fa-step-forward:before {
  content: "\f051";
}
.fa-eject:before {
  content: "\f052";
}
.fa-chevron-left:before {
  content: "\f053";
}
.fa-chevron-right:before {
  content: "\f054";
}
.fa-plus-circle:before {
  content: "\f055";
}
.fa-minus-circle:before {
  content: "\f056";
}
.fa-times-circle:before {
  content: "\f057";
}
.fa-check-circle:before {
  content: "\f058";
}
.fa-question-circle:before {
  content: "\f059";
}
.fa-info-circle:before {
  content: "\f05a";
}
.fa-crosshairs:before {
  content: "\f05b";
}
.fa-times-circle-o:before {
  content: "\f05c";
}
.fa-check-circle-o:before {
  content: "\f05d";
}
.fa-ban:before {
  content: "\f05e";
}
.fa-arrow-left:before {
  content: "\f060";
}
.fa-arrow-right:before {
  content: "\f061";
}
.fa-arrow-up:before {
  content: "\f062";
}
.fa-arrow-down:before {
  content: "\f063";
}
.fa-mail-forward:before,
.fa-share:before {
  content: "\f064";
}
.fa-expand:before {
  content: "\f065";
}
.fa-compress:before {
  content: "\f066";
}
.fa-plus:before {
  content: "\f067";
}
.fa-minus:before {
  content: "\f068";
}
.fa-asterisk:before {
  content: "\f069";
}
.fa-exclamation-circle:before {
  content: "\f06a";
}
.fa-gift:before {
  content: "\f06b";
}
.fa-leaf:before {
  content: "\f06c";
}
.fa-fire:before {
  content: "\f06d";
}
.fa-eye:before {
  content: "\f06e";
}
.fa-eye-slash:before {
  content: "\f070";
}
.fa-warning:before,
.fa-exclamation-triangle:before {
  content: "\f071";
}
.fa-plane:before {
  content: "\f072";
}
.fa-calendar:before {
  content: "\f073";
}
.fa-random:before {
  content: "\f074";
}
.fa-comment:before {
  content: "\f075";
}
.fa-magnet:before {
  content: "\f076";
}
.fa-chevron-up:before {
  content: "\f077";
}
.fa-chevron-down:before {
  content: "\f078";
}
.fa-retweet:before {
  content: "\f079";
}
.fa-shopping-cart:before {
  content: "\f07a";
}
.fa-folder:before {
  content: "\f07b";
}
.fa-folder-open:before {
  content: "\f07c";
}
.fa-arrows-v:before {
  content: "\f07d";
}
.fa-arrows-h:before {
  content: "\f07e";
}
.fa-bar-chart-o:before,
.fa-bar-chart:before {
  content: "\f080";
}
.fa-twitter-square:before {
  content: "\f081";
}
.fa-facebook-square:before {
  content: "\f082";
}
.fa-camera-retro:before {
  content: "\f083";
}
.fa-key:before {
  content: "\f084";
}
.fa-gears:before,
.fa-cogs:before {
  content: "\f085";
}
.fa-comments:before {
  content: "\f086";
}
.fa-thumbs-o-up:before {
  content: "\f087";
}
.fa-thumbs-o-down:before {
  content: "\f088";
}
.fa-star-half:before {
  content: "\f089";
}
.fa-heart-o:before {
  content: "\f08a";
}
.fa-sign-out:before {
  content: "\f08b";
}
.fa-linkedin-square:before {
  content: "\f08c";
}
.fa-thumb-tack:before {
  content: "\f08d";
}
.fa-external-link:before {
  content: "\f08e";
}
.fa-sign-in:before {
  content: "\f090";
}
.fa-trophy:before {
  content: "\f091";
}
.fa-github-square:before {
  content: "\f092";
}
.fa-upload:before {
  content: "\f093";
}
.fa-lemon-o:before {
  content: "\f094";
}
.fa-phone:before {
  content: "\f095";
}
.fa-square-o:before {
  content: "\f096";
}
.fa-bookmark-o:before {
  content: "\f097";
}
.fa-phone-square:before {
  content: "\f098";
}
.fa-twitter:before {
  content: "\f099";
}
.fa-facebook:before {
  content: "\f09a";
}
.fa-github:before {
  content: "\f09b";
}
.fa-unlock:before {
  content: "\f09c";
}
.fa-credit-card:before {
  content: "\f09d";
}
.fa-rss:before {
  content: "\f09e";
}
.fa-hdd-o:before {
  content: "\f0a0";
}
.fa-bullhorn:before {
  content: "\f0a1";
}
.fa-bell:before {
  content: "\f0f3";
}
.fa-certificate:before {
  content: "\f0a3";
}
.fa-hand-o-right:before {
  content: "\f0a4";
}
.fa-hand-o-left:before {
  content: "\f0a5";
}
.fa-hand-o-up:before {
  content: "\f0a6";
}
.fa-hand-o-down:before {
  content: "\f0a7";
}
.fa-arrow-circle-left:before {
  content: "\f0a8";
}
.fa-arrow-circle-right:before {
  content: "\f0a9";
}
.fa-arrow-circle-up:before {
  content: "\f0aa";
}
.fa-arrow-circle-down:before {
  content: "\f0ab";
}
.fa-globe:before {
  content: "\f0ac";
}
.fa-wrench:before {
  content: "\f0ad";
}
.fa-tasks:before {
  content: "\f0ae";
}
.fa-filter:before {
  content: "\f0b0";
}
.fa-briefcase:before {
  content: "\f0b1";
}
.fa-arrows-alt:before {
  content: "\f0b2";
}
.fa-group:before,
.fa-users:before {
  content: "\f0c0";
}
.fa-chain:before,
.fa-link:before {
  content: "\f0c1";
}
.fa-cloud:before {
  content: "\f0c2";
}
.fa-flask:before {
  content: "\f0c3";
}
.fa-cut:before,
.fa-scissors:before {
  content: "\f0c4";
}
.fa-copy:before,
.fa-files-o:before {
  content: "\f0c5";
}
.fa-paperclip:before {
  content: "\f0c6";
}
.fa-save:before,
.fa-floppy-o:before {
  content: "\f0c7";
}
.fa-square:before {
  content: "\f0c8";
}
.fa-navicon:before,
.fa-reorder:before,
.fa-bars:before {
  content: "\f0c9";
}
.fa-list-ul:before {
  content: "\f0ca";
}
.fa-list-ol:before {
  content: "\f0cb";
}
.fa-strikethrough:before {
  content: "\f0cc";
}
.fa-underline:before {
  content: "\f0cd";
}
.fa-table:before {
  content: "\f0ce";
}
.fa-magic:before {
  content: "\f0d0";
}
.fa-truck:before {
  content: "\f0d1";
}
.fa-pinterest:before {
  content: "\f0d2";
}
.fa-pinterest-square:before {
  content: "\f0d3";
}
.fa-google-plus-square:before {
  content: "\f0d4";
}
.fa-google-plus:before {
  content: "\f0d5";
}
.fa-money:before {
  content: "\f0d6";
}
.fa-caret-down:before {
  content: "\f0d7";
}
.fa-caret-up:before {
  content: "\f0d8";
}
.fa-caret-left:before {
  content: "\f0d9";
}
.fa-caret-right:before {
  content: "\f0da";
}
.fa-columns:before {
  content: "\f0db";
}
.fa-unsorted:before,
.fa-sort:before {
  content: "\f0dc";
}
.fa-sort-down:before,
.fa-sort-desc:before {
  content: "\f0dd";
}
.fa-sort-up:before,
.fa-sort-asc:before {
  content: "\f0de";
}
.fa-envelope:before {
  content: "\f0e0";
}
.fa-linkedin:before {
  content: "\f0e1";
}
.fa-rotate-left:before,
.fa-undo:before {
  content: "\f0e2";
}
.fa-legal:before,
.fa-gavel:before {
  content: "\f0e3";
}
.fa-dashboard:before,
.fa-tachometer:before {
  content: "\f0e4";
}
.fa-comment-o:before {
  content: "\f0e5";
}
.fa-comments-o:before {
  content: "\f0e6";
}
.fa-flash:before,
.fa-bolt:before {
  content: "\f0e7";
}
.fa-sitemap:before {
  content: "\f0e8";
}
.fa-umbrella:before {
  content: "\f0e9";
}
.fa-paste:before,
.fa-clipboard:before {
  content: "\f0ea";
}
.fa-lightbulb-o:before {
  content: "\f0eb";
}
.fa-exchange:before {
  content: "\f0ec";
}
.fa-cloud-download:before {
  content: "\f0ed";
}
.fa-cloud-upload:before {
  content: "\f0ee";
}
.fa-user-md:before {
  content: "\f0f0";
}
.fa-stethoscope:before {
  content: "\f0f1";
}
.fa-suitcase:before {
  content: "\f0f2";
}
.fa-bell-o:before {
  content: "\f0a2";
}
.fa-coffee:before {
  content: "\f0f4";
}
.fa-cutlery:before {
  content: "\f0f5";
}
.fa-file-text-o:before {
  content: "\f0f6";
}
.fa-building-o:before {
  content: "\f0f7";
}
.fa-hospital-o:before {
  content: "\f0f8";
}
.fa-ambulance:before {
  content: "\f0f9";
}
.fa-medkit:before {
  content: "\f0fa";
}
.fa-fighter-jet:before {
  content: "\f0fb";
}
.fa-beer:before {
  content: "\f0fc";
}
.fa-h-square:before {
  content: "\f0fd";
}
.fa-plus-square:before {
  content: "\f0fe";
}
.fa-angle-double-left:before {
  content: "\f100";
}
.fa-angle-double-right:before {
  content: "\f101";
}
.fa-angle-double-up:before {
  content: "\f102";
}
.fa-angle-double-down:before {
  content: "\f103";
}
.fa-angle-left:before {
  content: "\f104";
}
.fa-angle-right:before {
  content: "\f105";
}
.fa-angle-up:before {
  content: "\f106";
}
.fa-angle-down:before {
  content: "\f107";
}
.fa-desktop:before {
  content: "\f108";
}
.fa-laptop:before {
  content: "\f109";
}
.fa-tablet:before {
  content: "\f10a";
}
.fa-mobile-phone:before,
.fa-mobile:before {
  content: "\f10b";
}
.fa-circle-o:before {
  content: "\f10c";
}
.fa-quote-left:before {
  content: "\f10d";
}
.fa-quote-right:before {
  content: "\f10e";
}
.fa-spinner:before {
  content: "\f110";
}
.fa-circle:before {
  content: "\f111";
}
.fa-mail-reply:before,
.fa-reply:before {
  content: "\f112";
}
.fa-github-alt:before {
  content: "\f113";
}
.fa-folder-o:before {
  content: "\f114";
}
.fa-folder-open-o:before {
  content: "\f115";
}
.fa-smile-o:before {
  content: "\f118";
}
.fa-frown-o:before {
  content: "\f119";
}
.fa-meh-o:before {
  content: "\f11a";
}
.fa-gamepad:before {
  content: "\f11b";
}
.fa-keyboard-o:before {
  content: "\f11c";
}
.fa-flag-o:before {
  content: "\f11d";
}
.fa-flag-checkered:before {
  content: "\f11e";
}
.fa-terminal:before {
  content: "\f120";
}
.fa-code:before {
  content: "\f121";
}
.fa-mail-reply-all:before,
.fa-reply-all:before {
  content: "\f122";
}
.fa-star-half-empty:before,
.fa-star-half-full:before,
.fa-star-half-o:before {
  content: "\f123";
}
.fa-location-arrow:before {
  content: "\f124";
}
.fa-crop:before {
  content: "\f125";
}
.fa-code-fork:before {
  content: "\f126";
}
.fa-unlink:before,
.fa-chain-broken:before {
  content: "\f127";
}
.fa-question:before {
  content: "\f128";
}
.fa-info:before {
  content: "\f129";
}
.fa-exclamation:before {
  content: "\f12a";
}
.fa-superscript:before {
  content: "\f12b";
}
.fa-subscript:before {
  content: "\f12c";
}
.fa-eraser:before {
  content: "\f12d";
}
.fa-puzzle-piece:before {
  content: "\f12e";
}
.fa-microphone:before {
  content: "\f130";
}
.fa-microphone-slash:before {
  content: "\f131";
}
.fa-shield:before {
  content: "\f132";
}
.fa-calendar-o:before {
  content: "\f133";
}
.fa-fire-extinguisher:before {
  content: "\f134";
}
.fa-rocket:before {
  content: "\f135";
}
.fa-maxcdn:before {
  content: "\f136";
}
.fa-chevron-circle-left:before {
  content: "\f137";
}
.fa-chevron-circle-right:before {
  content: "\f138";
}
.fa-chevron-circle-up:before {
  content: "\f139";
}
.fa-chevron-circle-down:before {
  content: "\f13a";
}
.fa-html5:before {
  content: "\f13b";
}
.fa-css3:before {
  content: "\f13c";
}
.fa-anchor:before {
  content: "\f13d";
}
.fa-unlock-alt:before {
  content: "\f13e";
}
.fa-bullseye:before {
  content: "\f140";
}
.fa-ellipsis-h:before {
  content: "\f141";
}
.fa-ellipsis-v:before {
  content: "\f142";
}
.fa-rss-square:before {
  content: "\f143";
}
.fa-play-circle:before {
  content: "\f144";
}
.fa-ticket:before {
  content: "\f145";
}
.fa-minus-square:before {
  content: "\f146";
}
.fa-minus-square-o:before {
  content: "\f147";
}
.fa-level-up:before {
  content: "\f148";
}
.fa-level-down:before {
  content: "\f149";
}
.fa-check-square:before {
  content: "\f14a";
}
.fa-pencil-square:before {
  content: "\f14b";
}
.fa-external-link-square:before {
  content: "\f14c";
}
.fa-share-square:before {
  content: "\f14d";
}
.fa-compass:before {
  content: "\f14e";
}
.fa-toggle-down:before,
.fa-caret-square-o-down:before {
  content: "\f150";
}
.fa-toggle-up:before,
.fa-caret-square-o-up:before {
  content: "\f151";
}
.fa-toggle-right:before,
.fa-caret-square-o-right:before {
  content: "\f152";
}
.fa-euro:before,
.fa-eur:before {
  content: "\f153";
}
.fa-gbp:before {
  content: "\f154";
}
.fa-dollar:before,
.fa-usd:before {
  content: "\f155";
}
.fa-rupee:before,
.fa-inr:before {
  content: "\f156";
}
.fa-cny:before,
.fa-rmb:before,
.fa-yen:before,
.fa-jpy:before {
  content: "\f157";
}
.fa-ruble:before,
.fa-rouble:before,
.fa-rub:before {
  content: "\f158";
}
.fa-won:before,
.fa-krw:before {
  content: "\f159";
}
.fa-bitcoin:before,
.fa-btc:before {
  content: "\f15a";
}
.fa-file:before {
  content: "\f15b";
}
.fa-file-text:before {
  content: "\f15c";
}
.fa-sort-alpha-asc:before {
  content: "\f15d";
}
.fa-sort-alpha-desc:before {
  content: "\f15e";
}
.fa-sort-amount-asc:before {
  content: "\f160";
}
.fa-sort-amount-desc:before {
  content: "\f161";
}
.fa-sort-numeric-asc:before {
  content: "\f162";
}
.fa-sort-numeric-desc:before {
  content: "\f163";
}
.fa-thumbs-up:before {
  content: "\f164";
}
.fa-thumbs-down:before {
  content: "\f165";
}
.fa-youtube-square:before {
  content: "\f166";
}
.fa-youtube:before {
  content: "\f167";
}
.fa-xing:before {
  content: "\f168";
}
.fa-xing-square:before {
  content: "\f169";
}
.fa-youtube-play:before {
  content: "\f16a";
}
.fa-dropbox:before {
  content: "\f16b";
}
.fa-stack-overflow:before {
  content: "\f16c";
}
.fa-instagram:before {
  content: "\f16d";
}
.fa-flickr:before {
  content: "\f16e";
}
.fa-adn:before {
  content: "\f170";
}
.fa-bitbucket:before {
  content: "\f171";
}
.fa-bitbucket-square:before {
  content: "\f172";
}
.fa-tumblr:before {
  content: "\f173";
}
.fa-tumblr-square:before {
  content: "\f174";
}
.fa-long-arrow-down:before {
  content: "\f175";
}
.fa-long-arrow-up:before {
  content: "\f176";
}
.fa-long-arrow-left:before {
  content: "\f177";
}
.fa-long-arrow-right:before {
  content: "\f178";
}
.fa-apple:before {
  content: "\f179";
}
.fa-windows:before {
  content: "\f17a";
}
.fa-android:before {
  content: "\f17b";
}
.fa-linux:before {
  content: "\f17c";
}
.fa-dribbble:before {
  content: "\f17d";
}
.fa-skype:before {
  content: "\f17e";
}
.fa-foursquare:before {
  content: "\f180";
}
.fa-trello:before {
  content: "\f181";
}
.fa-female:before {
  content: "\f182";
}
.fa-male:before {
  content: "\f183";
}
.fa-gittip:before {
  content: "\f184";
}
.fa-sun-o:before {
  content: "\f185";
}
.fa-moon-o:before {
  content: "\f186";
}
.fa-archive:before {
  content: "\f187";
}
.fa-bug:before {
  content: "\f188";
}
.fa-vk:before {
  content: "\f189";
}
.fa-weibo:before {
  content: "\f18a";
}
.fa-renren:before {
  content: "\f18b";
}
.fa-pagelines:before {
  content: "\f18c";
}
.fa-stack-exchange:before {
  content: "\f18d";
}
.fa-arrow-circle-o-right:before {
  content: "\f18e";
}
.fa-arrow-circle-o-left:before {
  content: "\f190";
}
.fa-toggle-left:before,
.fa-caret-square-o-left:before {
  content: "\f191";
}
.fa-dot-circle-o:before {
  content: "\f192";
}
.fa-wheelchair:before {
  content: "\f193";
}
.fa-vimeo-square:before {
  content: "\f194";
}
.fa-turkish-lira:before,
.fa-try:before {
  content: "\f195";
}
.fa-plus-square-o:before {
  content: "\f196";
}
.fa-space-shuttle:before {
  content: "\f197";
}
.fa-slack:before {
  content: "\f198";
}
.fa-envelope-square:before {
  content: "\f199";
}
.fa-wordpress:before {
  content: "\f19a";
}
.fa-openid:before {
  content: "\f19b";
}
.fa-institution:before,
.fa-bank:before,
.fa-university:before {
  content: "\f19c";
}
.fa-mortar-board:before,
.fa-graduation-cap:before {
  content: "\f19d";
}
.fa-yahoo:before {
  content: "\f19e";
}
.fa-google:before {
  content: "\f1a0";
}
.fa-reddit:before {
  content: "\f1a1";
}
.fa-reddit-square:before {
  content: "\f1a2";
}
.fa-stumbleupon-circle:before {
  content: "\f1a3";
}
.fa-stumbleupon:before {
  content: "\f1a4";
}
.fa-delicious:before {
  content: "\f1a5";
}
.fa-digg:before {
  content: "\f1a6";
}
.fa-pied-piper:before {
  content: "\f1a7";
}
.fa-pied-piper-alt:before {
  content: "\f1a8";
}
.fa-drupal:before {
  content: "\f1a9";
}
.fa-joomla:before {
  content: "\f1aa";
}
.fa-language:before {
  content: "\f1ab";
}
.fa-fax:before {
  content: "\f1ac";
}
.fa-building:before {
  content: "\f1ad";
}
.fa-child:before {
  content: "\f1ae";
}
.fa-paw:before {
  content: "\f1b0";
}
.fa-spoon:before {
  content: "\f1b1";
}
.fa-cube:before {
  content: "\f1b2";
}
.fa-cubes:before {
  content: "\f1b3";
}
.fa-behance:before {
  content: "\f1b4";
}
.fa-behance-square:before {
  content: "\f1b5";
}
.fa-steam:before {
  content: "\f1b6";
}
.fa-steam-square:before {
  content: "\f1b7";
}
.fa-recycle:before {
  content: "\f1b8";
}
.fa-automobile:before,
.fa-car:before {
  content: "\f1b9";
}
.fa-cab:before,
.fa-taxi:before {
  content: "\f1ba";
}
.fa-tree:before {
  content: "\f1bb";
}
.fa-spotify:before {
  content: "\f1bc";
}
.fa-deviantart:before {
  content: "\f1bd";
}
.fa-soundcloud:before {
  content: "\f1be";
}
.fa-database:before {
  content: "\f1c0";
}
.fa-file-pdf-o:before {
  content: "\f1c1";
}
.fa-file-word-o:before {
  content: "\f1c2";
}
.fa-file-excel-o:before {
  content: "\f1c3";
}
.fa-file-powerpoint-o:before {
  content: "\f1c4";
}
.fa-file-photo-o:before,
.fa-file-picture-o:before,
.fa-file-image-o:before {
  content: "\f1c5";
}
.fa-file-zip-o:before,
.fa-file-archive-o:before {
  content: "\f1c6";
}
.fa-file-sound-o:before,
.fa-file-audio-o:before {
  content: "\f1c7";
}
.fa-file-movie-o:before,
.fa-file-video-o:before {
  content: "\f1c8";
}
.fa-file-code-o:before {
  content: "\f1c9";
}
.fa-vine:before {
  content: "\f1ca";
}
.fa-codepen:before {
  content: "\f1cb";
}
.fa-jsfiddle:before {
  content: "\f1cc";
}
.fa-life-bouy:before,
.fa-life-buoy:before,
.fa-life-saver:before,
.fa-support:before,
.fa-life-ring:before {
  content: "\f1cd";
}
.fa-circle-o-notch:before {
  content: "\f1ce";
}
.fa-ra:before,
.fa-rebel:before {
  content: "\f1d0";
}
.fa-ge:before,
.fa-empire:before {
  content: "\f1d1";
}
.fa-git-square:before {
  content: "\f1d2";
}
.fa-git:before {
  content: "\f1d3";
}
.fa-hacker-news:before {
  content: "\f1d4";
}
.fa-tencent-weibo:before {
  content: "\f1d5";
}
.fa-qq:before {
  content: "\f1d6";
}
.fa-wechat:before,
.fa-weixin:before {
  content: "\f1d7";
}
.fa-send:before,
.fa-paper-plane:before {
  content: "\f1d8";
}
.fa-send-o:before,
.fa-paper-plane-o:before {
  content: "\f1d9";
}
.fa-history:before {
  content: "\f1da";
}
.fa-circle-thin:before {
  content: "\f1db";
}
.fa-header:before {
  content: "\f1dc";
}
.fa-paragraph:before {
  content: "\f1dd";
}
.fa-sliders:before {
  content: "\f1de";
}
.fa-share-alt:before {
  content: "\f1e0";
}
.fa-share-alt-square:before {
  content: "\f1e1";
}
.fa-bomb:before {
  content: "\f1e2";
}
.fa-soccer-ball-o:before,
.fa-futbol-o:before {
  content: "\f1e3";
}
.fa-tty:before {
  content: "\f1e4";
}
.fa-binoculars:before {
  content: "\f1e5";
}
.fa-plug:before {
  content: "\f1e6";
}
.fa-slideshare:before {
  content: "\f1e7";
}
.fa-twitch:before {
  content: "\f1e8";
}
.fa-yelp:before {
  content: "\f1e9";
}
.fa-newspaper-o:before {
  content: "\f1ea";
}
.fa-wifi:before {
  content: "\f1eb";
}
.fa-calculator:before {
  content: "\f1ec";
}
.fa-paypal:before {
  content: "\f1ed";
}
.fa-google-wallet:before {
  content: "\f1ee";
}
.fa-cc-visa:before {
  content: "\f1f0";
}
.fa-cc-mastercard:before {
  content: "\f1f1";
}
.fa-cc-discover:before {
  content: "\f1f2";
}
.fa-cc-amex:before {
  content: "\f1f3";
}
.fa-cc-paypal:before {
  content: "\f1f4";
}
.fa-cc-stripe:before {
  content: "\f1f5";
}
.fa-bell-slash:before {
  content: "\f1f6";
}
.fa-bell-slash-o:before {
  content: "\f1f7";
}
.fa-trash:before {
  content: "\f1f8";
}
.fa-copyright:before {
  content: "\f1f9";
}
.fa-at:before {
  content: "\f1fa";
}
.fa-eyedropper:before {
  content: "\f1fb";
}
.fa-paint-brush:before {
  content: "\f1fc";
}
.fa-birthday-cake:before {
  content: "\f1fd";
}
.fa-area-chart:before {
  content: "\f1fe";
}
.fa-pie-chart:before {
  content: "\f200";
}
.fa-line-chart:before {
  content: "\f201";
}
.fa-lastfm:before {
  content: "\f202";
}
.fa-lastfm-square:before {
  content: "\f203";
}
.fa-toggle-off:before {
  content: "\f204";
}
.fa-toggle-on:before {
  content: "\f205";
}
.fa-bicycle:before {
  content: "\f206";
}
.fa-bus:before {
  content: "\f207";
}
.fa-ioxhost:before {
  content: "\f208";
}
.fa-angellist:before {
  content: "\f209";
}
.fa-cc:before {
  content: "\f20a";
}
.fa-shekel:before,
.fa-sheqel:before,
.fa-ils:before {
  content: "\f20b";
}
.fa-meanpath:before {
  content: "\f20c";
}
/*!
*
* IPython base
*
*/
.modal.fade .modal-dialog {
  -webkit-transform: translate(0, 0);
  -ms-transform: translate(0, 0);
  -o-transform: translate(0, 0);
  transform: translate(0, 0);
}
code {
  color: #000;
}
pre {
  font-size: inherit;
  line-height: inherit;
}
label {
  font-weight: normal;
}
/* Make the page background atleast 100% the height of the view port */
/* Make the page itself atleast 70% the height of the view port */
.border-box-sizing {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
.corner-all {
  border-radius: 2px;
}
.no-padding {
  padding: 0px;
}
/* Flexible box model classes */
/* Taken from Alex Russell http://infrequently.org/2009/08/css-3-progress/ */
/* This file is a compatability layer.  It allows the usage of flexible box 
model layouts accross multiple browsers, including older browsers.  The newest,
universal implementation of the flexible box model is used when available (see
`Modern browsers` comments below).  Browsers that are known to implement this 
new spec completely include:

    Firefox 28.0+
    Chrome 29.0+
    Internet Explorer 11+ 
    Opera 17.0+

Browsers not listed, including Safari, are supported via the styling under the
`Old browsers` comments below.
*/
.hbox {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
.hbox > * {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
}
.vbox {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
.vbox > * {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
}
.hbox.reverse,
.vbox.reverse,
.reverse {
  /* Old browsers */
  -webkit-box-direction: reverse;
  -moz-box-direction: reverse;
  box-direction: reverse;
  /* Modern browsers */
  flex-direction: row-reverse;
}
.hbox.box-flex0,
.vbox.box-flex0,
.box-flex0 {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
  width: auto;
}
.hbox.box-flex1,
.vbox.box-flex1,
.box-flex1 {
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
.hbox.box-flex,
.vbox.box-flex,
.box-flex {
  /* Old browsers */
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
.hbox.box-flex2,
.vbox.box-flex2,
.box-flex2 {
  /* Old browsers */
  -webkit-box-flex: 2;
  -moz-box-flex: 2;
  box-flex: 2;
  /* Modern browsers */
  flex: 2;
}
.box-group1 {
  /*  Deprecated */
  -webkit-box-flex-group: 1;
  -moz-box-flex-group: 1;
  box-flex-group: 1;
}
.box-group2 {
  /* Deprecated */
  -webkit-box-flex-group: 2;
  -moz-box-flex-group: 2;
  box-flex-group: 2;
}
.hbox.start,
.vbox.start,
.start {
  /* Old browsers */
  -webkit-box-pack: start;
  -moz-box-pack: start;
  box-pack: start;
  /* Modern browsers */
  justify-content: flex-start;
}
.hbox.end,
.vbox.end,
.end {
  /* Old browsers */
  -webkit-box-pack: end;
  -moz-box-pack: end;
  box-pack: end;
  /* Modern browsers */
  justify-content: flex-end;
}
.hbox.center,
.vbox.center,
.center {
  /* Old browsers */
  -webkit-box-pack: center;
  -moz-box-pack: center;
  box-pack: center;
  /* Modern browsers */
  justify-content: center;
}
.hbox.baseline,
.vbox.baseline,
.baseline {
  /* Old browsers */
  -webkit-box-pack: baseline;
  -moz-box-pack: baseline;
  box-pack: baseline;
  /* Modern browsers */
  justify-content: baseline;
}
.hbox.stretch,
.vbox.stretch,
.stretch {
  /* Old browsers */
  -webkit-box-pack: stretch;
  -moz-box-pack: stretch;
  box-pack: stretch;
  /* Modern browsers */
  justify-content: stretch;
}
.hbox.align-start,
.vbox.align-start,
.align-start {
  /* Old browsers */
  -webkit-box-align: start;
  -moz-box-align: start;
  box-align: start;
  /* Modern browsers */
  align-items: flex-start;
}
.hbox.align-end,
.vbox.align-end,
.align-end {
  /* Old browsers */
  -webkit-box-align: end;
  -moz-box-align: end;
  box-align: end;
  /* Modern browsers */
  align-items: flex-end;
}
.hbox.align-center,
.vbox.align-center,
.align-center {
  /* Old browsers */
  -webkit-box-align: center;
  -moz-box-align: center;
  box-align: center;
  /* Modern browsers */
  align-items: center;
}
.hbox.align-baseline,
.vbox.align-baseline,
.align-baseline {
  /* Old browsers */
  -webkit-box-align: baseline;
  -moz-box-align: baseline;
  box-align: baseline;
  /* Modern browsers */
  align-items: baseline;
}
.hbox.align-stretch,
.vbox.align-stretch,
.align-stretch {
  /* Old browsers */
  -webkit-box-align: stretch;
  -moz-box-align: stretch;
  box-align: stretch;
  /* Modern browsers */
  align-items: stretch;
}
div.error {
  margin: 2em;
  text-align: center;
}
div.error > h1 {
  font-size: 500%;
  line-height: normal;
}
div.error > p {
  font-size: 200%;
  line-height: normal;
}
div.traceback-wrapper {
  text-align: left;
  max-width: 800px;
  margin: auto;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
body {
  background-color: #fff;
  /* This makes sure that the body covers the entire window and needs to
       be in a different element than the display: box in wrapper below */
  position: absolute;
  left: 0px;
  right: 0px;
  top: 0px;
  bottom: 0px;
  overflow: visible;
}
body > #header {
  /* Initially hidden to prevent FLOUC */
  display: none;
  background-color: #fff;
  /* Display over codemirror */
  position: relative;
  z-index: 100;
}
body > #header #header-container {
  padding-bottom: 5px;
  padding-top: 5px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
body > #header .header-bar {
  width: 100%;
  height: 1px;
  background: #e7e7e7;
  margin-bottom: -1px;
}
@media print {
  body > #header {
    display: none !important;
  }
}
#header-spacer {
  width: 100%;
  visibility: hidden;
}
@media print {
  #header-spacer {
    display: none;
  }
}
#ipython_notebook {
  padding-left: 0px;
  padding-top: 1px;
  padding-bottom: 1px;
}
@media (max-width: 991px) {
  #ipython_notebook {
    margin-left: 10px;
  }
}
[dir="rtl"] #ipython_notebook {
  float: right !important;
}
#noscript {
  width: auto;
  padding-top: 16px;
  padding-bottom: 16px;
  text-align: center;
  font-size: 22px;
  color: red;
  font-weight: bold;
}
#ipython_notebook img {
  height: 28px;
}
#site {
  width: 100%;
  display: none;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  overflow: auto;
}
@media print {
  #site {
    height: auto !important;
  }
}
/* Smaller buttons */
.ui-button .ui-button-text {
  padding: 0.2em 0.8em;
  font-size: 77%;
}
input.ui-button {
  padding: 0.3em 0.9em;
}
span#login_widget {
  float: right;
}
span#login_widget > .button,
#logout {
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
span#login_widget > .button:focus,
#logout:focus,
span#login_widget > .button.focus,
#logout.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
span#login_widget > .button:hover,
#logout:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
span#login_widget > .button:active,
#logout:active,
span#login_widget > .button.active,
#logout.active,
.open > .dropdown-togglespan#login_widget > .button,
.open > .dropdown-toggle#logout {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
span#login_widget > .button:active:hover,
#logout:active:hover,
span#login_widget > .button.active:hover,
#logout.active:hover,
.open > .dropdown-togglespan#login_widget > .button:hover,
.open > .dropdown-toggle#logout:hover,
span#login_widget > .button:active:focus,
#logout:active:focus,
span#login_widget > .button.active:focus,
#logout.active:focus,
.open > .dropdown-togglespan#login_widget > .button:focus,
.open > .dropdown-toggle#logout:focus,
span#login_widget > .button:active.focus,
#logout:active.focus,
span#login_widget > .button.active.focus,
#logout.active.focus,
.open > .dropdown-togglespan#login_widget > .button.focus,
.open > .dropdown-toggle#logout.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
span#login_widget > .button:active,
#logout:active,
span#login_widget > .button.active,
#logout.active,
.open > .dropdown-togglespan#login_widget > .button,
.open > .dropdown-toggle#logout {
  background-image: none;
}
span#login_widget > .button.disabled:hover,
#logout.disabled:hover,
span#login_widget > .button[disabled]:hover,
#logout[disabled]:hover,
fieldset[disabled] span#login_widget > .button:hover,
fieldset[disabled] #logout:hover,
span#login_widget > .button.disabled:focus,
#logout.disabled:focus,
span#login_widget > .button[disabled]:focus,
#logout[disabled]:focus,
fieldset[disabled] span#login_widget > .button:focus,
fieldset[disabled] #logout:focus,
span#login_widget > .button.disabled.focus,
#logout.disabled.focus,
span#login_widget > .button[disabled].focus,
#logout[disabled].focus,
fieldset[disabled] span#login_widget > .button.focus,
fieldset[disabled] #logout.focus {
  background-color: #fff;
  border-color: #ccc;
}
span#login_widget > .button .badge,
#logout .badge {
  color: #fff;
  background-color: #333;
}
.nav-header {
  text-transform: none;
}
#header > span {
  margin-top: 10px;
}
.modal_stretch .modal-dialog {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  min-height: 80vh;
}
.modal_stretch .modal-dialog .modal-body {
  max-height: calc(100vh - 200px);
  overflow: auto;
  flex: 1;
}
@media (min-width: 768px) {
  .modal .modal-dialog {
    width: 700px;
  }
}
@media (min-width: 768px) {
  select.form-control {
    margin-left: 12px;
    margin-right: 12px;
  }
}
/*!
*
* IPython auth
*
*/
.center-nav {
  display: inline-block;
  margin-bottom: -4px;
}
/*!
*
* IPython tree view
*
*/
/* We need an invisible input field on top of the sentense*/
/* "Drag file onto the list ..." */
.alternate_upload {
  background-color: none;
  display: inline;
}
.alternate_upload.form {
  padding: 0;
  margin: 0;
}
.alternate_upload input.fileinput {
  text-align: center;
  vertical-align: middle;
  display: inline;
  opacity: 0;
  z-index: 2;
  width: 12ex;
  margin-right: -12ex;
}
.alternate_upload .btn-upload {
  height: 22px;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
[dir="rtl"] #tabs li {
  float: right;
}
ul#tabs {
  margin-bottom: 4px;
}
[dir="rtl"] ul#tabs {
  margin-right: 0px;
}
ul#tabs a {
  padding-top: 6px;
  padding-bottom: 4px;
}
ul.breadcrumb a:focus,
ul.breadcrumb a:hover {
  text-decoration: none;
}
ul.breadcrumb i.icon-home {
  font-size: 16px;
  margin-right: 4px;
}
ul.breadcrumb span {
  color: #5e5e5e;
}
.list_toolbar {
  padding: 4px 0 4px 0;
  vertical-align: middle;
}
.list_toolbar .tree-buttons {
  padding-top: 1px;
}
[dir="rtl"] .list_toolbar .tree-buttons {
  float: left !important;
}
[dir="rtl"] .list_toolbar .pull-right {
  padding-top: 1px;
  float: left !important;
}
[dir="rtl"] .list_toolbar .pull-left {
  float: right !important;
}
.dynamic-buttons {
  padding-top: 3px;
  display: inline-block;
}
.list_toolbar [class*="span"] {
  min-height: 24px;
}
.list_header {
  font-weight: bold;
  background-color: #EEE;
}
.list_placeholder {
  font-weight: bold;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
}
.list_container {
  margin-top: 4px;
  margin-bottom: 20px;
  border: 1px solid #ddd;
  border-radius: 2px;
}
.list_container > div {
  border-bottom: 1px solid #ddd;
}
.list_container > div:hover .list-item {
  background-color: red;
}
.list_container > div:last-child {
  border: none;
}
.list_item:hover .list_item {
  background-color: #ddd;
}
.list_item a {
  text-decoration: none;
}
.list_item:hover {
  background-color: #fafafa;
}
.list_header > div,
.list_item > div {
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
  line-height: 22px;
}
.list_header > div input,
.list_item > div input {
  margin-right: 7px;
  margin-left: 14px;
  vertical-align: baseline;
  line-height: 22px;
  position: relative;
  top: -1px;
}
.list_header > div .item_link,
.list_item > div .item_link {
  margin-left: -1px;
  vertical-align: baseline;
  line-height: 22px;
}
.new-file input[type=checkbox] {
  visibility: hidden;
}
.item_name {
  line-height: 22px;
  height: 24px;
}
.item_icon {
  font-size: 14px;
  color: #5e5e5e;
  margin-right: 7px;
  margin-left: 7px;
  line-height: 22px;
  vertical-align: baseline;
}
.item_buttons {
  line-height: 1em;
  margin-left: -5px;
}
.item_buttons .btn,
.item_buttons .btn-group,
.item_buttons .input-group {
  float: left;
}
.item_buttons > .btn,
.item_buttons > .btn-group,
.item_buttons > .input-group {
  margin-left: 5px;
}
.item_buttons .btn {
  min-width: 13ex;
}
.item_buttons .running-indicator {
  padding-top: 4px;
  color: #5cb85c;
}
.item_buttons .kernel-name {
  padding-top: 4px;
  color: #5bc0de;
  margin-right: 7px;
  float: left;
}
.toolbar_info {
  height: 24px;
  line-height: 24px;
}
.list_item input:not([type=checkbox]) {
  padding-top: 3px;
  padding-bottom: 3px;
  height: 22px;
  line-height: 14px;
  margin: 0px;
}
.highlight_text {
  color: blue;
}
#project_name {
  display: inline-block;
  padding-left: 7px;
  margin-left: -2px;
}
#project_name > .breadcrumb {
  padding: 0px;
  margin-bottom: 0px;
  background-color: transparent;
  font-weight: bold;
}
#tree-selector {
  padding-right: 0px;
}
[dir="rtl"] #tree-selector a {
  float: right;
}
#button-select-all {
  min-width: 50px;
}
#select-all {
  margin-left: 7px;
  margin-right: 2px;
}
.menu_icon {
  margin-right: 2px;
}
.tab-content .row {
  margin-left: 0px;
  margin-right: 0px;
}
.folder_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f114";
}
.folder_icon:before.pull-left {
  margin-right: .3em;
}
.folder_icon:before.pull-right {
  margin-left: .3em;
}
.notebook_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f02d";
  position: relative;
  top: -1px;
}
.notebook_icon:before.pull-left {
  margin-right: .3em;
}
.notebook_icon:before.pull-right {
  margin-left: .3em;
}
.running_notebook_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f02d";
  position: relative;
  top: -1px;
  color: #5cb85c;
}
.running_notebook_icon:before.pull-left {
  margin-right: .3em;
}
.running_notebook_icon:before.pull-right {
  margin-left: .3em;
}
.file_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f016";
  position: relative;
  top: -2px;
}
.file_icon:before.pull-left {
  margin-right: .3em;
}
.file_icon:before.pull-right {
  margin-left: .3em;
}
#notebook_toolbar .pull-right {
  padding-top: 0px;
  margin-right: -1px;
}
ul#new-menu {
  left: auto;
  right: 0;
}
[dir="rtl"] #new-menu {
  text-align: right;
}
.kernel-menu-icon {
  padding-right: 12px;
  width: 24px;
  content: "\f096";
}
.kernel-menu-icon:before {
  content: "\f096";
}
.kernel-menu-icon-current:before {
  content: "\f00c";
}
#tab_content {
  padding-top: 20px;
}
#running .panel-group .panel {
  margin-top: 3px;
  margin-bottom: 1em;
}
#running .panel-group .panel .panel-heading {
  background-color: #EEE;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
  line-height: 22px;
}
#running .panel-group .panel .panel-heading a:focus,
#running .panel-group .panel .panel-heading a:hover {
  text-decoration: none;
}
#running .panel-group .panel .panel-body {
  padding: 0px;
}
#running .panel-group .panel .panel-body .list_container {
  margin-top: 0px;
  margin-bottom: 0px;
  border: 0px;
  border-radius: 0px;
}
#running .panel-group .panel .panel-body .list_container .list_item {
  border-bottom: 1px solid #ddd;
}
#running .panel-group .panel .panel-body .list_container .list_item:last-child {
  border-bottom: 0px;
}
[dir="rtl"] #running .col-sm-8 {
  float: right !important;
}
.delete-button {
  display: none;
}
.duplicate-button {
  display: none;
}
.rename-button {
  display: none;
}
.shutdown-button {
  display: none;
}
.dynamic-instructions {
  display: inline-block;
  padding-top: 4px;
}
/*!
*
* IPython text editor webapp
*
*/
.selected-keymap i.fa {
  padding: 0px 5px;
}
.selected-keymap i.fa:before {
  content: "\f00c";
}
#mode-menu {
  overflow: auto;
  max-height: 20em;
}
.edit_app #header {
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
.edit_app #menubar .navbar {
  /* Use a negative 1 bottom margin, so the border overlaps the border of the
    header */
  margin-bottom: -1px;
}
.dirty-indicator {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator.pull-left {
  margin-right: .3em;
}
.dirty-indicator.pull-right {
  margin-left: .3em;
}
.dirty-indicator-dirty {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator-dirty.pull-left {
  margin-right: .3em;
}
.dirty-indicator-dirty.pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator-clean.pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean.pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f00c";
}
.dirty-indicator-clean:before.pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean:before.pull-right {
  margin-left: .3em;
}
#filename {
  font-size: 16pt;
  display: table;
  padding: 0px 5px;
}
#current-mode {
  padding-left: 5px;
  padding-right: 5px;
}
#texteditor-backdrop {
  padding-top: 20px;
  padding-bottom: 20px;
}
@media not print {
  #texteditor-backdrop {
    background-color: #EEE;
  }
}
@media print {
  #texteditor-backdrop #texteditor-container .CodeMirror-gutter,
  #texteditor-backdrop #texteditor-container .CodeMirror-gutters {
    background-color: #fff;
  }
}
@media not print {
  #texteditor-backdrop #texteditor-container .CodeMirror-gutter,
  #texteditor-backdrop #texteditor-container .CodeMirror-gutters {
    background-color: #fff;
  }
}
@media not print {
  #texteditor-backdrop #texteditor-container {
    padding: 0px;
    background-color: #fff;
    -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
    box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  }
}
/*!
*
* IPython notebook
*
*/
/* CSS font colors for translated ANSI colors. */
.ansibold {
  font-weight: bold;
}
/* use dark versions for foreground, to improve visibility */
.ansiblack {
  color: black;
}
.ansired {
  color: darkred;
}
.ansigreen {
  color: darkgreen;
}
.ansiyellow {
  color: #c4a000;
}
.ansiblue {
  color: darkblue;
}
.ansipurple {
  color: darkviolet;
}
.ansicyan {
  color: steelblue;
}
.ansigray {
  color: gray;
}
/* and light for background, for the same reason */
.ansibgblack {
  background-color: black;
}
.ansibgred {
  background-color: red;
}
.ansibggreen {
  background-color: green;
}
.ansibgyellow {
  background-color: yellow;
}
.ansibgblue {
  background-color: blue;
}
.ansibgpurple {
  background-color: magenta;
}
.ansibgcyan {
  background-color: cyan;
}
.ansibggray {
  background-color: gray;
}
div.cell {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  border-radius: 2px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  border-width: 1px;
  border-style: solid;
  border-color: transparent;
  width: 100%;
  padding: 5px;
  /* This acts as a spacer between cells, that is outside the border */
  margin: 0px;
  outline: none;
  border-left-width: 1px;
  padding-left: 5px;
  background: linear-gradient(to right, transparent -40px, transparent 1px, transparent 1px, transparent 100%);
}
div.cell.jupyter-soft-selected {
  border-left-color: #90CAF9;
  border-left-color: #E3F2FD;
  border-left-width: 1px;
  padding-left: 5px;
  border-right-color: #E3F2FD;
  border-right-width: 1px;
  background: #E3F2FD;
}
@media print {
  div.cell.jupyter-soft-selected {
    border-color: transparent;
  }
}
div.cell.selected {
  border-color: #ababab;
  border-left-width: 0px;
  padding-left: 6px;
  background: linear-gradient(to right, #42A5F5 -40px, #42A5F5 5px, transparent 5px, transparent 100%);
}
@media print {
  div.cell.selected {
    border-color: transparent;
  }
}
div.cell.selected.jupyter-soft-selected {
  border-left-width: 0;
  padding-left: 6px;
  background: linear-gradient(to right, #42A5F5 -40px, #42A5F5 7px, #E3F2FD 7px, #E3F2FD 100%);
}
.edit_mode div.cell.selected {
  border-color: #66BB6A;
  border-left-width: 0px;
  padding-left: 6px;
  background: linear-gradient(to right, #66BB6A -40px, #66BB6A 5px, transparent 5px, transparent 100%);
}
@media print {
  .edit_mode div.cell.selected {
    border-color: transparent;
  }
}
.prompt {
  /* This needs to be wide enough for 3 digit prompt numbers: In[100]: */
  min-width: 14ex;
  /* This padding is tuned to match the padding on the CodeMirror editor. */
  padding: 0.4em;
  margin: 0px;
  font-family: monospace;
  text-align: right;
  /* This has to match that of the the CodeMirror class line-height below */
  line-height: 1.21429em;
  /* Don't highlight prompt number selection */
  -webkit-touch-callout: none;
  -webkit-user-select: none;
  -khtml-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
  /* Use default cursor */
  cursor: default;
}
@media (max-width: 540px) {
  .prompt {
    text-align: left;
  }
}
div.inner_cell {
  min-width: 0;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
/* input_area and input_prompt must match in top border and margin for alignment */
div.input_area {
  border: 1px solid #cfcfcf;
  border-radius: 2px;
  background: #f7f7f7;
  line-height: 1.21429em;
}
/* This is needed so that empty prompt areas can collapse to zero height when there
   is no content in the output_subarea and the prompt. The main purpose of this is
   to make sure that empty JavaScript output_subareas have no height. */
div.prompt:empty {
  padding-top: 0;
  padding-bottom: 0;
}
div.unrecognized_cell {
  padding: 5px 5px 5px 0px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
div.unrecognized_cell .inner_cell {
  border-radius: 2px;
  padding: 5px;
  font-weight: bold;
  color: red;
  border: 1px solid #cfcfcf;
  background: #eaeaea;
}
div.unrecognized_cell .inner_cell a {
  color: inherit;
  text-decoration: none;
}
div.unrecognized_cell .inner_cell a:hover {
  color: inherit;
  text-decoration: none;
}
@media (max-width: 540px) {
  div.unrecognized_cell > div.prompt {
    display: none;
  }
}
div.code_cell {
  /* avoid page breaking on code cells when printing */
}
@media print {
  div.code_cell {
    page-break-inside: avoid;
  }
}
/* any special styling for code cells that are currently running goes here */
div.input {
  page-break-inside: avoid;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.input {
    /* Old browsers */
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-box-align: stretch;
    display: -moz-box;
    -moz-box-orient: vertical;
    -moz-box-align: stretch;
    display: box;
    box-orient: vertical;
    box-align: stretch;
    /* Modern browsers */
    display: flex;
    flex-direction: column;
    align-items: stretch;
  }
}
/* input_area and input_prompt must match in top border and margin for alignment */
div.input_prompt {
  color: #303F9F;
  border-top: 1px solid transparent;
}
div.input_area > div.highlight {
  margin: 0.4em;
  border: none;
  padding: 0px;
  background-color: transparent;
}
div.input_area > div.highlight > pre {
  margin: 0px;
  border: none;
  padding: 0px;
  background-color: transparent;
}
/* The following gets added to the <head> if it is detected that the user has a
 * monospace font with inconsistent normal/bold/italic height.  See
 * notebookmain.js.  Such fonts will have keywords vertically offset with
 * respect to the rest of the text.  The user should select a better font.
 * See: https://github.com/ipython/ipython/issues/1503
 *
 * .CodeMirror span {
 *      vertical-align: bottom;
 * }
 */
.CodeMirror {
  line-height: 1.21429em;
  /* Changed from 1em to our global default */
  font-size: 14px;
  height: auto;
  /* Changed to auto to autogrow */
  background: none;
  /* Changed from white to allow our bg to show through */
}
.CodeMirror-scroll {
  /*  The CodeMirror docs are a bit fuzzy on if overflow-y should be hidden or visible.*/
  /*  We have found that if it is visible, vertical scrollbars appear with font size changes.*/
  overflow-y: hidden;
  overflow-x: auto;
}
.CodeMirror-lines {
  /* In CM2, this used to be 0.4em, but in CM3 it went to 4px. We need the em value because */
  /* we have set a different line-height and want this to scale with that. */
  padding: 0.4em;
}
.CodeMirror-linenumber {
  padding: 0 8px 0 4px;
}
.CodeMirror-gutters {
  border-bottom-left-radius: 2px;
  border-top-left-radius: 2px;
}
.CodeMirror pre {
  /* In CM3 this went to 4px from 0 in CM2. We need the 0 value because of how we size */
  /* .CodeMirror-lines */
  padding: 0;
  border: 0;
  border-radius: 0;
}
/*

Original style from softwaremaniacs.org (c) Ivan Sagalaev <Maniac@SoftwareManiacs.Org>
Adapted from GitHub theme

*/
.highlight-base {
  color: #000;
}
.highlight-variable {
  color: #000;
}
.highlight-variable-2 {
  color: #1a1a1a;
}
.highlight-variable-3 {
  color: #333333;
}
.highlight-string {
  color: #BA2121;
}
.highlight-comment {
  color: #408080;
  font-style: italic;
}
.highlight-number {
  color: #080;
}
.highlight-atom {
  color: #88F;
}
.highlight-keyword {
  color: #008000;
  font-weight: bold;
}
.highlight-builtin {
  color: #008000;
}
.highlight-error {
  color: #f00;
}
.highlight-operator {
  color: #AA22FF;
  font-weight: bold;
}
.highlight-meta {
  color: #AA22FF;
}
/* previously not defined, copying from default codemirror */
.highlight-def {
  color: #00f;
}
.highlight-string-2 {
  color: #f50;
}
.highlight-qualifier {
  color: #555;
}
.highlight-bracket {
  color: #997;
}
.highlight-tag {
  color: #170;
}
.highlight-attribute {
  color: #00c;
}
.highlight-header {
  color: blue;
}
.highlight-quote {
  color: #090;
}
.highlight-link {
  color: #00c;
}
/* apply the same style to codemirror */
.cm-s-ipython span.cm-keyword {
  color: #008000;
  font-weight: bold;
}
.cm-s-ipython span.cm-atom {
  color: #88F;
}
.cm-s-ipython span.cm-number {
  color: #080;
}
.cm-s-ipython span.cm-def {
  color: #00f;
}
.cm-s-ipython span.cm-variable {
  color: #000;
}
.cm-s-ipython span.cm-operator {
  color: #AA22FF;
  font-weight: bold;
}
.cm-s-ipython span.cm-variable-2 {
  color: #1a1a1a;
}
.cm-s-ipython span.cm-variable-3 {
  color: #333333;
}
.cm-s-ipython span.cm-comment {
  color: #408080;
  font-style: italic;
}
.cm-s-ipython span.cm-string {
  color: #BA2121;
}
.cm-s-ipython span.cm-string-2 {
  color: #f50;
}
.cm-s-ipython span.cm-meta {
  color: #AA22FF;
}
.cm-s-ipython span.cm-qualifier {
  color: #555;
}
.cm-s-ipython span.cm-builtin {
  color: #008000;
}
.cm-s-ipython span.cm-bracket {
  color: #997;
}
.cm-s-ipython span.cm-tag {
  color: #170;
}
.cm-s-ipython span.cm-attribute {
  color: #00c;
}
.cm-s-ipython span.cm-header {
  color: blue;
}
.cm-s-ipython span.cm-quote {
  color: #090;
}
.cm-s-ipython span.cm-link {
  color: #00c;
}
.cm-s-ipython span.cm-error {
  color: #f00;
}
.cm-s-ipython span.cm-tab {
  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAMCAYAAAAkuj5RAAAAAXNSR0IArs4c6QAAAGFJREFUSMft1LsRQFAQheHPowAKoACx3IgEKtaEHujDjORSgWTH/ZOdnZOcM/sgk/kFFWY0qV8foQwS4MKBCS3qR6ixBJvElOobYAtivseIE120FaowJPN75GMu8j/LfMwNjh4HUpwg4LUAAAAASUVORK5CYII=);
  background-position: right;
  background-repeat: no-repeat;
}
div.output_wrapper {
  /* this position must be relative to enable descendents to be absolute within it */
  position: relative;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  z-index: 1;
}
/* class for the output area when it should be height-limited */
div.output_scroll {
  /* ideally, this would be max-height, but FF barfs all over that */
  height: 24em;
  /* FF needs this *and the wrapper* to specify full width, or it will shrinkwrap */
  width: 100%;
  overflow: auto;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 2px 8px rgba(0, 0, 0, 0.8);
  box-shadow: inset 0 2px 8px rgba(0, 0, 0, 0.8);
  display: block;
}
/* output div while it is collapsed */
div.output_collapsed {
  margin: 0px;
  padding: 0px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
div.out_prompt_overlay {
  height: 100%;
  padding: 0px 0.4em;
  position: absolute;
  border-radius: 2px;
}
div.out_prompt_overlay:hover {
  /* use inner shadow to get border that is computed the same on WebKit/FF */
  -webkit-box-shadow: inset 0 0 1px #000;
  box-shadow: inset 0 0 1px #000;
  background: rgba(240, 240, 240, 0.5);
}
div.output_prompt {
  color: #D84315;
}
/* This class is the outer container of all output sections. */
div.output_area {
  padding: 0px;
  page-break-inside: avoid;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
div.output_area .MathJax_Display {
  text-align: left !important;
}
div.output_area .rendered_html table {
  margin-left: 0;
  margin-right: 0;
}
div.output_area .rendered_html img {
  margin-left: 0;
  margin-right: 0;
}
div.output_area img,
div.output_area svg {
  max-width: 100%;
  height: auto;
}
div.output_area img.unconfined,
div.output_area svg.unconfined {
  max-width: none;
}
/* This is needed to protect the pre formating from global settings such
   as that of bootstrap */
.output {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.output_area {
    /* Old browsers */
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-box-align: stretch;
    display: -moz-box;
    -moz-box-orient: vertical;
    -moz-box-align: stretch;
    display: box;
    box-orient: vertical;
    box-align: stretch;
    /* Modern browsers */
    display: flex;
    flex-direction: column;
    align-items: stretch;
  }
}
div.output_area pre {
  margin: 0;
  padding: 0;
  border: 0;
  vertical-align: baseline;
  color: black;
  background-color: transparent;
  border-radius: 0;
}
/* This class is for the output subarea inside the output_area and after
   the prompt div. */
div.output_subarea {
  overflow-x: auto;
  padding: 0.4em;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
  max-width: calc(100% - 14ex);
}
div.output_scroll div.output_subarea {
  overflow-x: visible;
}
/* The rest of the output_* classes are for special styling of the different
   output types */
/* all text output has this class: */
div.output_text {
  text-align: left;
  color: #000;
  /* This has to match that of the the CodeMirror class line-height below */
  line-height: 1.21429em;
}
/* stdout/stderr are 'text' as well as 'stream', but execute_result/error are *not* streams */
div.output_stderr {
  background: #fdd;
  /* very light red background for stderr */
}
div.output_latex {
  text-align: left;
}
/* Empty output_javascript divs should have no height */
div.output_javascript:empty {
  padding: 0;
}
.js-error {
  color: darkred;
}
/* raw_input styles */
div.raw_input_container {
  line-height: 1.21429em;
  padding-top: 5px;
}
pre.raw_input_prompt {
  /* nothing needed here. */
}
input.raw_input {
  font-family: monospace;
  font-size: inherit;
  color: inherit;
  width: auto;
  /* make sure input baseline aligns with prompt */
  vertical-align: baseline;
  /* padding + margin = 0.5em between prompt and cursor */
  padding: 0em 0.25em;
  margin: 0em 0.25em;
}
input.raw_input:focus {
  box-shadow: none;
}
p.p-space {
  margin-bottom: 10px;
}
div.output_unrecognized {
  padding: 5px;
  font-weight: bold;
  color: red;
}
div.output_unrecognized a {
  color: inherit;
  text-decoration: none;
}
div.output_unrecognized a:hover {
  color: inherit;
  text-decoration: none;
}
.rendered_html {
  color: #000;
  /* any extras will just be numbers: */
}
.rendered_html em {
  font-style: italic;
}
.rendered_html strong {
  font-weight: bold;
}
.rendered_html u {
  text-decoration: underline;
}
.rendered_html :link {
  text-decoration: underline;
}
.rendered_html :visited {
  text-decoration: underline;
}
.rendered_html h1 {
  font-size: 185.7%;
  margin: 1.08em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h2 {
  font-size: 157.1%;
  margin: 1.27em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h3 {
  font-size: 128.6%;
  margin: 1.55em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h4 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h5 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
  font-style: italic;
}
.rendered_html h6 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
  font-style: italic;
}
.rendered_html h1:first-child {
  margin-top: 0.538em;
}
.rendered_html h2:first-child {
  margin-top: 0.636em;
}
.rendered_html h3:first-child {
  margin-top: 0.777em;
}
.rendered_html h4:first-child {
  margin-top: 1em;
}
.rendered_html h5:first-child {
  margin-top: 1em;
}
.rendered_html h6:first-child {
  margin-top: 1em;
}
.rendered_html ul {
  list-style: disc;
  margin: 0em 2em;
  padding-left: 0px;
}
.rendered_html ul ul {
  list-style: square;
  margin: 0em 2em;
}
.rendered_html ul ul ul {
  list-style: circle;
  margin: 0em 2em;
}
.rendered_html ol {
  list-style: decimal;
  margin: 0em 2em;
  padding-left: 0px;
}
.rendered_html ol ol {
  list-style: upper-alpha;
  margin: 0em 2em;
}
.rendered_html ol ol ol {
  list-style: lower-alpha;
  margin: 0em 2em;
}
.rendered_html ol ol ol ol {
  list-style: lower-roman;
  margin: 0em 2em;
}
.rendered_html ol ol ol ol ol {
  list-style: decimal;
  margin: 0em 2em;
}
.rendered_html * + ul {
  margin-top: 1em;
}
.rendered_html * + ol {
  margin-top: 1em;
}
.rendered_html hr {
  color: black;
  background-color: black;
}
.rendered_html pre {
  margin: 1em 2em;
}
.rendered_html pre,
.rendered_html code {
  border: 0;
  background-color: #fff;
  color: #000;
  font-size: 100%;
  padding: 0px;
}
.rendered_html blockquote {
  margin: 1em 2em;
}
.rendered_html table {
  margin-left: auto;
  margin-right: auto;
  border: 1px solid black;
  border-collapse: collapse;
}
.rendered_html tr,
.rendered_html th,
.rendered_html td {
  border: 1px solid black;
  border-collapse: collapse;
  margin: 1em 2em;
}
.rendered_html td,
.rendered_html th {
  text-align: left;
  vertical-align: middle;
  padding: 4px;
}
.rendered_html th {
  font-weight: bold;
}
.rendered_html * + table {
  margin-top: 1em;
}
.rendered_html p {
  text-align: left;
}
.rendered_html * + p {
  margin-top: 1em;
}
.rendered_html img {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.rendered_html * + img {
  margin-top: 1em;
}
.rendered_html img,
.rendered_html svg {
  max-width: 100%;
  height: auto;
}
.rendered_html img.unconfined,
.rendered_html svg.unconfined {
  max-width: none;
}
div.text_cell {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.text_cell > div.prompt {
    display: none;
  }
}
div.text_cell_render {
  /*font-family: "Helvetica Neue", Arial, Helvetica, Geneva, sans-serif;*/
  outline: none;
  resize: none;
  width: inherit;
  border-style: none;
  padding: 0.5em 0.5em 0.5em 0.4em;
  color: #000;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
a.anchor-link:link {
  text-decoration: none;
  padding: 0px 20px;
  visibility: hidden;
}
h1:hover .anchor-link,
h2:hover .anchor-link,
h3:hover .anchor-link,
h4:hover .anchor-link,
h5:hover .anchor-link,
h6:hover .anchor-link {
  visibility: visible;
}
.text_cell.rendered .input_area {
  display: none;
}
.text_cell.rendered .rendered_html {
  overflow-x: auto;
  overflow-y: hidden;
}
.text_cell.unrendered .text_cell_render {
  display: none;
}
.cm-header-1,
.cm-header-2,
.cm-header-3,
.cm-header-4,
.cm-header-5,
.cm-header-6 {
  font-weight: bold;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
}
.cm-header-1 {
  font-size: 185.7%;
}
.cm-header-2 {
  font-size: 157.1%;
}
.cm-header-3 {
  font-size: 128.6%;
}
.cm-header-4 {
  font-size: 110%;
}
.cm-header-5 {
  font-size: 100%;
  font-style: italic;
}
.cm-header-6 {
  font-size: 100%;
  font-style: italic;
}
/*!
*
* IPython notebook webapp
*
*/
@media (max-width: 767px) {
  .notebook_app {
    padding-left: 0px;
    padding-right: 0px;
  }
}
#ipython-main-app {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  height: 100%;
}
div#notebook_panel {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  height: 100%;
}
div#notebook {
  font-size: 14px;
  line-height: 20px;
  overflow-y: hidden;
  overflow-x: auto;
  width: 100%;
  /* This spaces the page away from the edge of the notebook area */
  padding-top: 20px;
  margin: 0px;
  outline: none;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  min-height: 100%;
}
@media not print {
  #notebook-container {
    padding: 15px;
    background-color: #fff;
    min-height: 0;
    -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
    box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  }
}
@media print {
  #notebook-container {
    width: 100%;
  }
}
div.ui-widget-content {
  border: 1px solid #ababab;
  outline: none;
}
pre.dialog {
  background-color: #f7f7f7;
  border: 1px solid #ddd;
  border-radius: 2px;
  padding: 0.4em;
  padding-left: 2em;
}
p.dialog {
  padding: 0.2em;
}
/* Word-wrap output correctly.  This is the CSS3 spelling, though Firefox seems
   to not honor it correctly.  Webkit browsers (Chrome, rekonq, Safari) do.
 */
pre,
code,
kbd,
samp {
  white-space: pre-wrap;
}
#fonttest {
  font-family: monospace;
}
p {
  margin-bottom: 0;
}
.end_space {
  min-height: 100px;
  transition: height .2s ease;
}
.notebook_app > #header {
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
@media not print {
  .notebook_app {
    background-color: #EEE;
  }
}
kbd {
  border-style: solid;
  border-width: 1px;
  box-shadow: none;
  margin: 2px;
  padding-left: 2px;
  padding-right: 2px;
  padding-top: 1px;
  padding-bottom: 1px;
}
/* CSS for the cell toolbar */
.celltoolbar {
  border: thin solid #CFCFCF;
  border-bottom: none;
  background: #EEE;
  border-radius: 2px 2px 0px 0px;
  width: 100%;
  height: 29px;
  padding-right: 4px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
  /* Old browsers */
  -webkit-box-pack: end;
  -moz-box-pack: end;
  box-pack: end;
  /* Modern browsers */
  justify-content: flex-end;
  display: -webkit-flex;
}
@media print {
  .celltoolbar {
    display: none;
  }
}
.ctb_hideshow {
  display: none;
  vertical-align: bottom;
}
/* ctb_show is added to the ctb_hideshow div to show the cell toolbar.
   Cell toolbars are only shown when the ctb_global_show class is also set.
*/
.ctb_global_show .ctb_show.ctb_hideshow {
  display: block;
}
.ctb_global_show .ctb_show + .input_area,
.ctb_global_show .ctb_show + div.text_cell_input,
.ctb_global_show .ctb_show ~ div.text_cell_render {
  border-top-right-radius: 0px;
  border-top-left-radius: 0px;
}
.ctb_global_show .ctb_show ~ div.text_cell_render {
  border: 1px solid #cfcfcf;
}
.celltoolbar {
  font-size: 87%;
  padding-top: 3px;
}
.celltoolbar select {
  display: block;
  width: 100%;
  height: 32px;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
  width: inherit;
  font-size: inherit;
  height: 22px;
  padding: 0px;
  display: inline-block;
}
.celltoolbar select:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.celltoolbar select::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.celltoolbar select:-ms-input-placeholder {
  color: #999;
}
.celltoolbar select::-webkit-input-placeholder {
  color: #999;
}
.celltoolbar select::-ms-expand {
  border: 0;
  background-color: transparent;
}
.celltoolbar select[disabled],
.celltoolbar select[readonly],
fieldset[disabled] .celltoolbar select {
  background-color: #eeeeee;
  opacity: 1;
}
.celltoolbar select[disabled],
fieldset[disabled] .celltoolbar select {
  cursor: not-allowed;
}
textarea.celltoolbar select {
  height: auto;
}
select.celltoolbar select {
  height: 30px;
  line-height: 30px;
}
textarea.celltoolbar select,
select[multiple].celltoolbar select {
  height: auto;
}
.celltoolbar label {
  margin-left: 5px;
  margin-right: 5px;
}
.completions {
  position: absolute;
  z-index: 110;
  overflow: hidden;
  border: 1px solid #ababab;
  border-radius: 2px;
  -webkit-box-shadow: 0px 6px 10px -1px #adadad;
  box-shadow: 0px 6px 10px -1px #adadad;
  line-height: 1;
}
.completions select {
  background: white;
  outline: none;
  border: none;
  padding: 0px;
  margin: 0px;
  overflow: auto;
  font-family: monospace;
  font-size: 110%;
  color: #000;
  width: auto;
}
.completions select option.context {
  color: #286090;
}
#kernel_logo_widget {
  float: right !important;
  float: right;
}
#kernel_logo_widget .current_kernel_logo {
  display: none;
  margin-top: -1px;
  margin-bottom: -1px;
  width: 32px;
  height: 32px;
}
#menubar {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  margin-top: 1px;
}
#menubar .navbar {
  border-top: 1px;
  border-radius: 0px 0px 2px 2px;
  margin-bottom: 0px;
}
#menubar .navbar-toggle {
  float: left;
  padding-top: 7px;
  padding-bottom: 7px;
  border: none;
}
#menubar .navbar-collapse {
  clear: left;
}
.nav-wrapper {
  border-bottom: 1px solid #e7e7e7;
}
i.menu-icon {
  padding-top: 4px;
}
ul#help_menu li a {
  overflow: hidden;
  padding-right: 2.2em;
}
ul#help_menu li a i {
  margin-right: -1.2em;
}
.dropdown-submenu {
  position: relative;
}
.dropdown-submenu > .dropdown-menu {
  top: 0;
  left: 100%;
  margin-top: -6px;
  margin-left: -1px;
}
.dropdown-submenu:hover > .dropdown-menu {
  display: block;
}
.dropdown-submenu > a:after {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  display: block;
  content: "\f0da";
  float: right;
  color: #333333;
  margin-top: 2px;
  margin-right: -10px;
}
.dropdown-submenu > a:after.pull-left {
  margin-right: .3em;
}
.dropdown-submenu > a:after.pull-right {
  margin-left: .3em;
}
.dropdown-submenu:hover > a:after {
  color: #262626;
}
.dropdown-submenu.pull-left {
  float: none;
}
.dropdown-submenu.pull-left > .dropdown-menu {
  left: -100%;
  margin-left: 10px;
}
#notification_area {
  float: right !important;
  float: right;
  z-index: 10;
}
.indicator_area {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
}
#kernel_indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
  border-left: 1px solid;
}
#kernel_indicator .kernel_indicator_name {
  padding-left: 5px;
  padding-right: 5px;
}
#modal_indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
}
#readonly-indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
  margin-top: 2px;
  margin-bottom: 0px;
  margin-left: 0px;
  margin-right: 0px;
  display: none;
}
.modal_indicator:before {
  width: 1.28571429em;
  text-align: center;
}
.edit_mode .modal_indicator:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f040";
}
.edit_mode .modal_indicator:before.pull-left {
  margin-right: .3em;
}
.edit_mode .modal_indicator:before.pull-right {
  margin-left: .3em;
}
.command_mode .modal_indicator:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: ' ';
}
.command_mode .modal_indicator:before.pull-left {
  margin-right: .3em;
}
.command_mode .modal_indicator:before.pull-right {
  margin-left: .3em;
}
.kernel_idle_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f10c";
}
.kernel_idle_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_idle_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_busy_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f111";
}
.kernel_busy_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_busy_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_dead_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f1e2";
}
.kernel_dead_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_dead_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_disconnected_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f127";
}
.kernel_disconnected_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_disconnected_icon:before.pull-right {
  margin-left: .3em;
}
.notification_widget {
  color: #777;
  z-index: 10;
  background: rgba(240, 240, 240, 0.5);
  margin-right: 4px;
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
.notification_widget:focus,
.notification_widget.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
.notification_widget:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.notification_widget:active,
.notification_widget.active,
.open > .dropdown-toggle.notification_widget {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.notification_widget:active:hover,
.notification_widget.active:hover,
.open > .dropdown-toggle.notification_widget:hover,
.notification_widget:active:focus,
.notification_widget.active:focus,
.open > .dropdown-toggle.notification_widget:focus,
.notification_widget:active.focus,
.notification_widget.active.focus,
.open > .dropdown-toggle.notification_widget.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
.notification_widget:active,
.notification_widget.active,
.open > .dropdown-toggle.notification_widget {
  background-image: none;
}
.notification_widget.disabled:hover,
.notification_widget[disabled]:hover,
fieldset[disabled] .notification_widget:hover,
.notification_widget.disabled:focus,
.notification_widget[disabled]:focus,
fieldset[disabled] .notification_widget:focus,
.notification_widget.disabled.focus,
.notification_widget[disabled].focus,
fieldset[disabled] .notification_widget.focus {
  background-color: #fff;
  border-color: #ccc;
}
.notification_widget .badge {
  color: #fff;
  background-color: #333;
}
.notification_widget.warning {
  color: #fff;
  background-color: #f0ad4e;
  border-color: #eea236;
}
.notification_widget.warning:focus,
.notification_widget.warning.focus {
  color: #fff;
  background-color: #ec971f;
  border-color: #985f0d;
}
.notification_widget.warning:hover {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.notification_widget.warning:active,
.notification_widget.warning.active,
.open > .dropdown-toggle.notification_widget.warning {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.notification_widget.warning:active:hover,
.notification_widget.warning.active:hover,
.open > .dropdown-toggle.notification_widget.warning:hover,
.notification_widget.warning:active:focus,
.notification_widget.warning.active:focus,
.open > .dropdown-toggle.notification_widget.warning:focus,
.notification_widget.warning:active.focus,
.notification_widget.warning.active.focus,
.open > .dropdown-toggle.notification_widget.warning.focus {
  color: #fff;
  background-color: #d58512;
  border-color: #985f0d;
}
.notification_widget.warning:active,
.notification_widget.warning.active,
.open > .dropdown-toggle.notification_widget.warning {
  background-image: none;
}
.notification_widget.warning.disabled:hover,
.notification_widget.warning[disabled]:hover,
fieldset[disabled] .notification_widget.warning:hover,
.notification_widget.warning.disabled:focus,
.notification_widget.warning[disabled]:focus,
fieldset[disabled] .notification_widget.warning:focus,
.notification_widget.warning.disabled.focus,
.notification_widget.warning[disabled].focus,
fieldset[disabled] .notification_widget.warning.focus {
  background-color: #f0ad4e;
  border-color: #eea236;
}
.notification_widget.warning .badge {
  color: #f0ad4e;
  background-color: #fff;
}
.notification_widget.success {
  color: #fff;
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.notification_widget.success:focus,
.notification_widget.success.focus {
  color: #fff;
  background-color: #449d44;
  border-color: #255625;
}
.notification_widget.success:hover {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.notification_widget.success:active,
.notification_widget.success.active,
.open > .dropdown-toggle.notification_widget.success {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.notification_widget.success:active:hover,
.notification_widget.success.active:hover,
.open > .dropdown-toggle.notification_widget.success:hover,
.notification_widget.success:active:focus,
.notification_widget.success.active:focus,
.open > .dropdown-toggle.notification_widget.success:focus,
.notification_widget.success:active.focus,
.notification_widget.success.active.focus,
.open > .dropdown-toggle.notification_widget.success.focus {
  color: #fff;
  background-color: #398439;
  border-color: #255625;
}
.notification_widget.success:active,
.notification_widget.success.active,
.open > .dropdown-toggle.notification_widget.success {
  background-image: none;
}
.notification_widget.success.disabled:hover,
.notification_widget.success[disabled]:hover,
fieldset[disabled] .notification_widget.success:hover,
.notification_widget.success.disabled:focus,
.notification_widget.success[disabled]:focus,
fieldset[disabled] .notification_widget.success:focus,
.notification_widget.success.disabled.focus,
.notification_widget.success[disabled].focus,
fieldset[disabled] .notification_widget.success.focus {
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.notification_widget.success .badge {
  color: #5cb85c;
  background-color: #fff;
}
.notification_widget.info {
  color: #fff;
  background-color: #5bc0de;
  border-color: #46b8da;
}
.notification_widget.info:focus,
.notification_widget.info.focus {
  color: #fff;
  background-color: #31b0d5;
  border-color: #1b6d85;
}
.notification_widget.info:hover {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.notification_widget.info:active,
.notification_widget.info.active,
.open > .dropdown-toggle.notification_widget.info {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.notification_widget.info:active:hover,
.notification_widget.info.active:hover,
.open > .dropdown-toggle.notification_widget.info:hover,
.notification_widget.info:active:focus,
.notification_widget.info.active:focus,
.open > .dropdown-toggle.notification_widget.info:focus,
.notification_widget.info:active.focus,
.notification_widget.info.active.focus,
.open > .dropdown-toggle.notification_widget.info.focus {
  color: #fff;
  background-color: #269abc;
  border-color: #1b6d85;
}
.notification_widget.info:active,
.notification_widget.info.active,
.open > .dropdown-toggle.notification_widget.info {
  background-image: none;
}
.notification_widget.info.disabled:hover,
.notification_widget.info[disabled]:hover,
fieldset[disabled] .notification_widget.info:hover,
.notification_widget.info.disabled:focus,
.notification_widget.info[disabled]:focus,
fieldset[disabled] .notification_widget.info:focus,
.notification_widget.info.disabled.focus,
.notification_widget.info[disabled].focus,
fieldset[disabled] .notification_widget.info.focus {
  background-color: #5bc0de;
  border-color: #46b8da;
}
.notification_widget.info .badge {
  color: #5bc0de;
  background-color: #fff;
}
.notification_widget.danger {
  color: #fff;
  background-color: #d9534f;
  border-color: #d43f3a;
}
.notification_widget.danger:focus,
.notification_widget.danger.focus {
  color: #fff;
  background-color: #c9302c;
  border-color: #761c19;
}
.notification_widget.danger:hover {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.notification_widget.danger:active,
.notification_widget.danger.active,
.open > .dropdown-toggle.notification_widget.danger {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.notification_widget.danger:active:hover,
.notification_widget.danger.active:hover,
.open > .dropdown-toggle.notification_widget.danger:hover,
.notification_widget.danger:active:focus,
.notification_widget.danger.active:focus,
.open > .dropdown-toggle.notification_widget.danger:focus,
.notification_widget.danger:active.focus,
.notification_widget.danger.active.focus,
.open > .dropdown-toggle.notification_widget.danger.focus {
  color: #fff;
  background-color: #ac2925;
  border-color: #761c19;
}
.notification_widget.danger:active,
.notification_widget.danger.active,
.open > .dropdown-toggle.notification_widget.danger {
  background-image: none;
}
.notification_widget.danger.disabled:hover,
.notification_widget.danger[disabled]:hover,
fieldset[disabled] .notification_widget.danger:hover,
.notification_widget.danger.disabled:focus,
.notification_widget.danger[disabled]:focus,
fieldset[disabled] .notification_widget.danger:focus,
.notification_widget.danger.disabled.focus,
.notification_widget.danger[disabled].focus,
fieldset[disabled] .notification_widget.danger.focus {
  background-color: #d9534f;
  border-color: #d43f3a;
}
.notification_widget.danger .badge {
  color: #d9534f;
  background-color: #fff;
}
div#pager {
  background-color: #fff;
  font-size: 14px;
  line-height: 20px;
  overflow: hidden;
  display: none;
  position: fixed;
  bottom: 0px;
  width: 100%;
  max-height: 50%;
  padding-top: 8px;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  /* Display over codemirror */
  z-index: 100;
  /* Hack which prevents jquery ui resizable from changing top. */
  top: auto !important;
}
div#pager pre {
  line-height: 1.21429em;
  color: #000;
  background-color: #f7f7f7;
  padding: 0.4em;
}
div#pager #pager-button-area {
  position: absolute;
  top: 8px;
  right: 20px;
}
div#pager #pager-contents {
  position: relative;
  overflow: auto;
  width: 100%;
  height: 100%;
}
div#pager #pager-contents #pager-container {
  position: relative;
  padding: 15px 0px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
div#pager .ui-resizable-handle {
  top: 0px;
  height: 8px;
  background: #f7f7f7;
  border-top: 1px solid #cfcfcf;
  border-bottom: 1px solid #cfcfcf;
  /* This injects handle bars (a short, wide = symbol) for 
        the resize handle. */
}
div#pager .ui-resizable-handle::after {
  content: '';
  top: 2px;
  left: 50%;
  height: 3px;
  width: 30px;
  margin-left: -15px;
  position: absolute;
  border-top: 1px solid #cfcfcf;
}
.quickhelp {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
  line-height: 1.8em;
}
.shortcut_key {
  display: inline-block;
  width: 21ex;
  text-align: right;
  font-family: monospace;
}
.shortcut_descr {
  display: inline-block;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
span.save_widget {
  margin-top: 6px;
}
span.save_widget span.filename {
  height: 1em;
  line-height: 1em;
  padding: 3px;
  margin-left: 16px;
  border: none;
  font-size: 146.5%;
  border-radius: 2px;
}
span.save_widget span.filename:hover {
  background-color: #e6e6e6;
}
span.checkpoint_status,
span.autosave_status {
  font-size: small;
}
@media (max-width: 767px) {
  span.save_widget {
    font-size: small;
  }
  span.checkpoint_status,
  span.autosave_status {
    display: none;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  span.checkpoint_status {
    display: none;
  }
  span.autosave_status {
    font-size: x-small;
  }
}
.toolbar {
  padding: 0px;
  margin-left: -5px;
  margin-top: 2px;
  margin-bottom: 5px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
.toolbar select,
.toolbar label {
  width: auto;
  vertical-align: middle;
  margin-right: 2px;
  margin-bottom: 0px;
  display: inline;
  font-size: 92%;
  margin-left: 0.3em;
  margin-right: 0.3em;
  padding: 0px;
  padding-top: 3px;
}
.toolbar .btn {
  padding: 2px 8px;
}
.toolbar .btn-group {
  margin-top: 0px;
  margin-left: 5px;
}
#maintoolbar {
  margin-bottom: -3px;
  margin-top: -8px;
  border: 0px;
  min-height: 27px;
  margin-left: 0px;
  padding-top: 11px;
  padding-bottom: 3px;
}
#maintoolbar .navbar-text {
  float: none;
  vertical-align: middle;
  text-align: right;
  margin-left: 5px;
  margin-right: 0px;
  margin-top: 0px;
}
.select-xs {
  height: 24px;
}
.pulse,
.dropdown-menu > li > a.pulse,
li.pulse > a.dropdown-toggle,
li.pulse.open > a.dropdown-toggle {
  background-color: #F37626;
  color: white;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
/** WARNING IF YOU ARE EDITTING THIS FILE, if this is a .css file, It has a lot
 * of chance of beeing generated from the ../less/[samename].less file, you can
 * try to get back the less file by reverting somme commit in history
 **/
/*
 * We'll try to get something pretty, so we
 * have some strange css to have the scroll bar on
 * the left with fix button on the top right of the tooltip
 */
@-moz-keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
@-webkit-keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
@-moz-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@-webkit-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
/*properties of tooltip after "expand"*/
.bigtooltip {
  overflow: auto;
  height: 200px;
  -webkit-transition-property: height;
  -webkit-transition-duration: 500ms;
  -moz-transition-property: height;
  -moz-transition-duration: 500ms;
  transition-property: height;
  transition-duration: 500ms;
}
/*properties of tooltip before "expand"*/
.smalltooltip {
  -webkit-transition-property: height;
  -webkit-transition-duration: 500ms;
  -moz-transition-property: height;
  -moz-transition-duration: 500ms;
  transition-property: height;
  transition-duration: 500ms;
  text-overflow: ellipsis;
  overflow: hidden;
  height: 80px;
}
.tooltipbuttons {
  position: absolute;
  padding-right: 15px;
  top: 0px;
  right: 0px;
}
.tooltiptext {
  /*avoid the button to overlap on some docstring*/
  padding-right: 30px;
}
.ipython_tooltip {
  max-width: 700px;
  /*fade-in animation when inserted*/
  -webkit-animation: fadeOut 400ms;
  -moz-animation: fadeOut 400ms;
  animation: fadeOut 400ms;
  -webkit-animation: fadeIn 400ms;
  -moz-animation: fadeIn 400ms;
  animation: fadeIn 400ms;
  vertical-align: middle;
  background-color: #f7f7f7;
  overflow: visible;
  border: #ababab 1px solid;
  outline: none;
  padding: 3px;
  margin: 0px;
  padding-left: 7px;
  font-family: monospace;
  min-height: 50px;
  -moz-box-shadow: 0px 6px 10px -1px #adadad;
  -webkit-box-shadow: 0px 6px 10px -1px #adadad;
  box-shadow: 0px 6px 10px -1px #adadad;
  border-radius: 2px;
  position: absolute;
  z-index: 1000;
}
.ipython_tooltip a {
  float: right;
}
.ipython_tooltip .tooltiptext pre {
  border: 0;
  border-radius: 0;
  font-size: 100%;
  background-color: #f7f7f7;
}
.pretooltiparrow {
  left: 0px;
  margin: 0px;
  top: -16px;
  width: 40px;
  height: 16px;
  overflow: hidden;
  position: absolute;
}
.pretooltiparrow:before {
  background-color: #f7f7f7;
  border: 1px #ababab solid;
  z-index: 11;
  content: "";
  position: absolute;
  left: 15px;
  top: 10px;
  width: 25px;
  height: 25px;
  -webkit-transform: rotate(45deg);
  -moz-transform: rotate(45deg);
  -ms-transform: rotate(45deg);
  -o-transform: rotate(45deg);
}
ul.typeahead-list i {
  margin-left: -10px;
  width: 18px;
}
ul.typeahead-list {
  max-height: 80vh;
  overflow: auto;
}
ul.typeahead-list > li > a {
  /** Firefox bug **/
  /* see https://github.com/jupyter/notebook/issues/559 */
  white-space: normal;
}
.cmd-palette .modal-body {
  padding: 7px;
}
.cmd-palette form {
  background: white;
}
.cmd-palette input {
  outline: none;
}
.no-shortcut {
  display: none;
}
.command-shortcut:before {
  content: "(command)";
  padding-right: 3px;
  color: #777777;
}
.edit-shortcut:before {
  content: "(edit)";
  padding-right: 3px;
  color: #777777;
}
#find-and-replace #replace-preview .match,
#find-and-replace #replace-preview .insert {
  background-color: #BBDEFB;
  border-color: #90CAF9;
  border-style: solid;
  border-width: 1px;
  border-radius: 0px;
}
#find-and-replace #replace-preview .replace .match {
  background-color: #FFCDD2;
  border-color: #EF9A9A;
  border-radius: 0px;
}
#find-and-replace #replace-preview .replace .insert {
  background-color: #C8E6C9;
  border-color: #A5D6A7;
  border-radius: 0px;
}
#find-and-replace #replace-preview {
  max-height: 60vh;
  overflow: auto;
}
#find-and-replace #replace-preview pre {
  padding: 5px 10px;
}
.terminal-app {
  background: #EEE;
}
.terminal-app #header {
  background: #fff;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
.terminal-app .terminal {
  width: 100%;
  float: left;
  font-family: monospace;
  color: white;
  background: black;
  padding: 0.4em;
  border-radius: 2px;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.4);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.4);
}
.terminal-app .terminal,
.terminal-app .terminal dummy-screen {
  line-height: 1em;
  font-size: 14px;
}
.terminal-app .terminal .xterm-rows {
  padding: 10px;
}
.terminal-app .terminal-cursor {
  color: black;
  background: white;
}
.terminal-app #terminado-container {
  margin-top: 20px;
}
/*# sourceMappingURL=style.min.css.map */
    </style>
<style type="text/css">
    .highlight .hll { background-color: #ffffcc }
.highlight  { background: #f8f8f8; }
.highlight .c { color: #408080; font-style: italic } /* Comment */
.highlight .err { border: 1px solid #FF0000 } /* Error */
.highlight .k { color: #008000; font-weight: bold } /* Keyword */
.highlight .o { color: #666666 } /* Operator */
.highlight .ch { color: #408080; font-style: italic } /* Comment.Hashbang */
.highlight .cm { color: #408080; font-style: italic } /* Comment.Multiline */
.highlight .cp { color: #BC7A00 } /* Comment.Preproc */
.highlight .cpf { color: #408080; font-style: italic } /* Comment.PreprocFile */
.highlight .c1 { color: #408080; font-style: italic } /* Comment.Single */
.highlight .cs { color: #408080; font-style: italic } /* Comment.Special */
.highlight .gd { color: #A00000 } /* Generic.Deleted */
.highlight .ge { font-style: italic } /* Generic.Emph */
.highlight .gr { color: #FF0000 } /* Generic.Error */
.highlight .gh { color: #000080; font-weight: bold } /* Generic.Heading */
.highlight .gi { color: #00A000 } /* Generic.Inserted */
.highlight .go { color: #888888 } /* Generic.Output */
.highlight .gp { color: #000080; font-weight: bold } /* Generic.Prompt */
.highlight .gs { font-weight: bold } /* Generic.Strong */
.highlight .gu { color: #800080; font-weight: bold } /* Generic.Subheading */
.highlight .gt { color: #0044DD } /* Generic.Traceback */
.highlight .kc { color: #008000; font-weight: bold } /* Keyword.Constant */
.highlight .kd { color: #008000; font-weight: bold } /* Keyword.Declaration */
.highlight .kn { color: #008000; font-weight: bold } /* Keyword.Namespace */
.highlight .kp { color: #008000 } /* Keyword.Pseudo */
.highlight .kr { color: #008000; font-weight: bold } /* Keyword.Reserved */
.highlight .kt { color: #B00040 } /* Keyword.Type */
.highlight .m { color: #666666 } /* Literal.Number */
.highlight .s { color: #BA2121 } /* Literal.String */
.highlight .na { color: #7D9029 } /* Name.Attribute */
.highlight .nb { color: #008000 } /* Name.Builtin */
.highlight .nc { color: #0000FF; font-weight: bold } /* Name.Class */
.highlight .no { color: #880000 } /* Name.Constant */
.highlight .nd { color: #AA22FF } /* Name.Decorator */
.highlight .ni { color: #999999; font-weight: bold } /* Name.Entity */
.highlight .ne { color: #D2413A; font-weight: bold } /* Name.Exception */
.highlight .nf { color: #0000FF } /* Name.Function */
.highlight .nl { color: #A0A000 } /* Name.Label */
.highlight .nn { color: #0000FF; font-weight: bold } /* Name.Namespace */
.highlight .nt { color: #008000; font-weight: bold } /* Name.Tag */
.highlight .nv { color: #19177C } /* Name.Variable */
.highlight .ow { color: #AA22FF; font-weight: bold } /* Operator.Word */
.highlight .w { color: #bbbbbb } /* Text.Whitespace */
.highlight .mb { color: #666666 } /* Literal.Number.Bin */
.highlight .mf { color: #666666 } /* Literal.Number.Float */
.highlight .mh { color: #666666 } /* Literal.Number.Hex */
.highlight .mi { color: #666666 } /* Literal.Number.Integer */
.highlight .mo { color: #666666 } /* Literal.Number.Oct */
.highlight .sa { color: #BA2121 } /* Literal.String.Affix */
.highlight .sb { color: #BA2121 } /* Literal.String.Backtick */
.highlight .sc { color: #BA2121 } /* Literal.String.Char */
.highlight .dl { color: #BA2121 } /* Literal.String.Delimiter */
.highlight .sd { color: #BA2121; font-style: italic } /* Literal.String.Doc */
.highlight .s2 { color: #BA2121 } /* Literal.String.Double */
.highlight .se { color: #BB6622; font-weight: bold } /* Literal.String.Escape */
.highlight .sh { color: #BA2121 } /* Literal.String.Heredoc */
.highlight .si { color: #BB6688; font-weight: bold } /* Literal.String.Interpol */
.highlight .sx { color: #008000 } /* Literal.String.Other */
.highlight .sr { color: #BB6688 } /* Literal.String.Regex */
.highlight .s1 { color: #BA2121 } /* Literal.String.Single */
.highlight .ss { color: #19177C } /* Literal.String.Symbol */
.highlight .bp { color: #008000 } /* Name.Builtin.Pseudo */
.highlight .fm { color: #0000FF } /* Name.Function.Magic */
.highlight .vc { color: #19177C } /* Name.Variable.Class */
.highlight .vg { color: #19177C } /* Name.Variable.Global */
.highlight .vi { color: #19177C } /* Name.Variable.Instance */
.highlight .vm { color: #19177C } /* Name.Variable.Magic */
.highlight .il { color: #666666 } /* Literal.Number.Integer.Long */
    </style>
<style type="text/css">
    
/* Temporary definitions which will become obsolete with Notebook release 5.0 */
.ansi-black-fg { color: #3E424D; }
.ansi-black-bg { background-color: #3E424D; }
.ansi-black-intense-fg { color: #282C36; }
.ansi-black-intense-bg { background-color: #282C36; }
.ansi-red-fg { color: #E75C58; }
.ansi-red-bg { background-color: #E75C58; }
.ansi-red-intense-fg { color: #B22B31; }
.ansi-red-intense-bg { background-color: #B22B31; }
.ansi-green-fg { color: #00A250; }
.ansi-green-bg { background-color: #00A250; }
.ansi-green-intense-fg { color: #007427; }
.ansi-green-intense-bg { background-color: #007427; }
.ansi-yellow-fg { color: #DDB62B; }
.ansi-yellow-bg { background-color: #DDB62B; }
.ansi-yellow-intense-fg { color: #B27D12; }
.ansi-yellow-intense-bg { background-color: #B27D12; }
.ansi-blue-fg { color: #208FFB; }
.ansi-blue-bg { background-color: #208FFB; }
.ansi-blue-intense-fg { color: #0065CA; }
.ansi-blue-intense-bg { background-color: #0065CA; }
.ansi-magenta-fg { color: #D160C4; }
.ansi-magenta-bg { background-color: #D160C4; }
.ansi-magenta-intense-fg { color: #A03196; }
.ansi-magenta-intense-bg { background-color: #A03196; }
.ansi-cyan-fg { color: #60C6C8; }
.ansi-cyan-bg { background-color: #60C6C8; }
.ansi-cyan-intense-fg { color: #258F8F; }
.ansi-cyan-intense-bg { background-color: #258F8F; }
.ansi-white-fg { color: #C5C1B4; }
.ansi-white-bg { background-color: #C5C1B4; }
.ansi-white-intense-fg { color: #A1A6B2; }
.ansi-white-intense-bg { background-color: #A1A6B2; }

.ansi-bold { font-weight: bold; }

    </style>


<style type="text/css">
/* Overrides of notebook CSS for static HTML export */
body {
  overflow: visible;
  padding: 8px;
}

div#notebook {
  overflow: visible;
  border-top: none;
}@media print {
  div.cell {
    display: block;
    page-break-inside: avoid;
  } 
  div.output_wrapper { 
    display: block;
    page-break-inside: avoid; 
  }
  div.output { 
    display: block;
    page-break-inside: avoid; 
  }
}
</style>

<!-- Custom stylesheet, it must be in the same directory as the html file -->
<link rel="stylesheet" href="custom.css">

<!-- Loading mathjax macro -->
<!-- Load mathjax -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS_HTML"></script>
    <!-- MathJax configuration -->
    <script type="text/x-mathjax-config">
    MathJax.Hub.Config({
        tex2jax: {
            inlineMath: [ ['$','$'], ["\\(","\\)"] ],
            displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
            processEscapes: true,
            processEnvironments: true
        },
        // Center justify equations in code and markdown cells. Elsewhere
        // we use CSS to left justify single line equations in code cells.
        displayAlign: 'center',
        "HTML-CSS": {
            styles: {'.MathJax_Display': {"margin": 0}},
            linebreaks: { automatic: true }
        }
    });
    </script>
    <!-- End of mathjax configuration --></head>
<body>
  <div tabindex="-1" id="notebook" class="border-box-sizing">
    <div class="container" id="notebook-container">

<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Machine-Learning-Engineer-Nanodegree">Machine Learning Engineer Nanodegree<a class="anchor-link" href="#Machine-Learning-Engineer-Nanodegree">&#182;</a></h1><h2 id="Reinforcement-Learning">Reinforcement Learning<a class="anchor-link" href="#Reinforcement-Learning">&#182;</a></h2><h2 id="Project:-Train-a-Smartcab-to-Drive">Project: Train a Smartcab to Drive<a class="anchor-link" href="#Project:-Train-a-Smartcab-to-Drive">&#182;</a></h2><p>Welcome to the fourth project of the Machine Learning Engineer Nanodegree! In this notebook, template code has already been provided for you to aid in your analysis of the <em>Smartcab</em> and your implemented learning algorithm. You will not need to modify the included code beyond what is requested. There will be questions that you must answer which relate to the project and the visualizations provided in the notebook. Each section where you will answer a question is preceded by a <strong>'Question X'</strong> header. Carefully read each question and provide thorough answers in the following text boxes that begin with <strong>'Answer:'</strong>. Your project submission will be evaluated based on your answers to each of the questions and the implementation you provide in <code>agent.py</code>.</p>
<blockquote><p><strong>Note:</strong> Code and Markdown cells can be executed using the <strong>Shift + Enter</strong> keyboard shortcut. In addition, Markdown cells can be edited by typically double-clicking the cell to enter edit mode.</p>
</blockquote>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<hr>
<h2 id="Getting-Started">Getting Started<a class="anchor-link" href="#Getting-Started">&#182;</a></h2><p>In this project, you will work towards constructing an optimized Q-Learning driving agent that will navigate a <em>Smartcab</em> through its environment towards a goal. Since the <em>Smartcab</em> is expected to drive passengers from one location to another, the driving agent will be evaluated on two very important metrics: <strong>Safety</strong> and <strong>Reliability</strong>. A driving agent that gets the <em>Smartcab</em> to its destination while running red lights or narrowly avoiding accidents would be considered <strong>unsafe</strong>. Similarly, a driving agent that frequently fails to reach the destination in time would be considered <strong>unreliable</strong>. Maximizing the driving agent's <strong>safety</strong> and <strong>reliability</strong> would ensure that <em>Smartcabs</em> have a permanent place in the transportation industry.</p>
<p><strong>Safety</strong> and <strong>Reliability</strong> are measured using a letter-grade system as follows:</p>
<table>
<thead><tr>
<th style="text-align:center">Grade</th>
<th style="text-align:center">Safety</th>
<th style="text-align:center">Reliability</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center">A+</td>
<td style="text-align:center">Agent commits no traffic violations,<br/>and always chooses the correct action.</td>
<td style="text-align:center">Agent reaches the destination in time<br />for 100% of trips.</td>
</tr>
<tr>
<td style="text-align:center">A</td>
<td style="text-align:center">Agent commits few minor traffic violations,<br/>such as failing to move on a green light.</td>
<td style="text-align:center">Agent reaches the destination on time<br />for at least 90% of trips.</td>
</tr>
<tr>
<td style="text-align:center">B</td>
<td style="text-align:center">Agent commits frequent minor traffic violations,<br/>such as failing to move on a green light.</td>
<td style="text-align:center">Agent reaches the destination on time<br />for at least 80% of trips.</td>
</tr>
<tr>
<td style="text-align:center">C</td>
<td style="text-align:center">Agent commits at least one major traffic violation,<br/> such as driving through a red light.</td>
<td style="text-align:center">Agent reaches the destination on time<br />for at least 70% of trips.</td>
</tr>
<tr>
<td style="text-align:center">D</td>
<td style="text-align:center">Agent causes at least one minor accident,<br/> such as turning left on green with oncoming traffic.</td>
<td style="text-align:center">Agent reaches the destination on time<br />for at least 60% of trips.</td>
</tr>
<tr>
<td style="text-align:center">F</td>
<td style="text-align:center">Agent causes at least one major accident,<br />such as driving through a red light with cross-traffic.</td>
<td style="text-align:center">Agent fails to reach the destination on time<br />for at least 60% of trips.</td>
</tr>
</tbody>
</table>
<p>To assist evaluating these important metrics, you will need to load visualization code that will be used later on in the project. Run the code cell below to import this code which is required for your analysis.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[2]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span></span><span class="c1"># Import the visualization code</span>
<span class="kn">import</span> <span class="nn">visuals</span> <span class="kn">as</span> <span class="nn">vs</span>

<span class="c1"># Pretty display for notebooks</span>
<span class="o">%</span><span class="k">matplotlib</span> inline
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Understand-the-World">Understand the World<a class="anchor-link" href="#Understand-the-World">&#182;</a></h3><p>Before starting to work on implementing your driving agent, it's necessary to first understand the world (environment) which the <em>Smartcab</em> and driving agent work in. One of the major components to building a self-learning agent is understanding the characteristics about the agent, which includes how the agent operates. To begin, simply run the <code>agent.py</code> agent code exactly how it is -- no need to make any additions whatsoever. Let the resulting simulation run for some time to see the various working components. Note that in the visual simulation (if enabled), the <strong>white vehicle</strong> is the <em>Smartcab</em>.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Question-1">Question 1<a class="anchor-link" href="#Question-1">&#182;</a></h3><p>In a few sentences, describe what you observe during the simulation when running the default <code>agent.py</code> agent code. Some things you could consider:</p>
<ul>
<li><em>Does the Smartcab move at all during the simulation?</em></li>
<li><em>What kind of rewards is the driving agent receiving?</em></li>
<li><em>How does the light changing color affect the rewards?</em>  </li>
</ul>
<p><strong>Hint:</strong> From the <code>/smartcab/</code> top-level directory (where this notebook is located), run the command</p>
<div class="highlight"><pre><span></span><span class="s1">&#39;python smartcab/agent.py&#39;</span>
</pre></div>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><strong>Answer:</strong></p>
<ol>
<li>The smartcab does not seems to be moving at all and is totally idled. </li>
<li>The driver agent is recieving different kind of rewards determined by traffic light state and oncoming traffic which are as below- <ul>
<li>When traffic light is red and the cab is idled , a positive reward is recieved. </li>
<li>When traffic light is green and there is no oncoming traffic, also the cab is idled then a negative reward is recieved.</li>
</ul>
</li>
<li>The light changing colour is affecting the rewards in the below manner-</li>
</ol>
<table>
<thead><tr>
<th style="text-align:center">Traffic light State</th>
<th style="text-align:center">Rewards State</th>
<th style="text-align:center">Reward Variation</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center">Green + no oncoming traffic</td>
<td style="text-align:center">Negative</td>
<td style="text-align:center">~-4.03 to ~-5.53</td>
</tr>
<tr>
<td style="text-align:center">Red + idled Traffic</td>
<td style="text-align:center">Positive</td>
<td style="text-align:center">~0.16 to ~2.35</td>
</tr>
</tbody>
</table>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Understand-the-Code">Understand the Code<a class="anchor-link" href="#Understand-the-Code">&#182;</a></h3><p>In addition to understanding the world, it is also necessary to understand the code itself that governs how the world, simulation, and so on operate. Attempting to create a driving agent would be difficult without having at least explored the <em>"hidden"</em> devices that make everything work. In the <code>/smartcab/</code> top-level directory, there are two folders: <code>/logs/</code> (which will be used later) and <code>/smartcab/</code>. Open the <code>/smartcab/</code> folder and explore each Python file included, then answer the following question.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Question-2">Question 2<a class="anchor-link" href="#Question-2">&#182;</a></h3><ul>
<li><em>In the </em><code>agent.py</code><em> Python file, choose three flags that can be set and explain how they change the simulation.</em></li>
<li><em>In the </em><code>environment.py</code><em> Python file, what Environment class function is called when an agent performs an action?</em></li>
<li><em>In the </em><code>simulator.py</code><em> Python file, what is the difference between the </em><code>'render_text()'</code><em> function and the </em><code>'render()'</code><em> function?</em></li>
<li><em>In the </em><code>planner.py</code><em> Python file, will the </em><code>'next_waypoint()</code><em> function consider the North-South or East-West direction first?</em></li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><strong>Answer:</strong></p>
<ol>
<li>Following are the three flags in the agent.py Python file- <ul>
<li><strong>learning</strong> This parameter takes boolean value to determine whether an agent is expected to learn (True) or he will simply choose non-specific action which is False.</li>
<li><strong>epsilon</strong> This parameter is random exploration factor. Any change in the value of epsilon will determine the learning behaviour of smart cab. On low paramaeter value, the smartcab will use its previous learnings to play safe and will not try to learn anything new. And on high parameter value it will take risks.</li>
<li><strong>alpha</strong> This parameter ranges in between 0 to 1. Here, 0 represents previous learnings only which means that the smart cab in not willing to implement any new learnings. Whereas 1 represents new learning only. And any value in between 0 to 1 means a mix of previous and new learnings. </li>
</ul>
</li>
<li>environment.py The <strong>act</strong> member class function is called when an agent performs an action and a reward is provided based on its actions.</li>
<li>simulator.py the 'render_text()' function is used for giving output into the command line window whereas 'render(
)' is used for giving output in the GUI.</li>
<li>planner.py checks whether the destination is at location or not. After that first it considers the East-West direction and then North-South direction.</li>
</ol>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<hr>
<h2 id="Implement-a-Basic-Driving-Agent">Implement a Basic Driving Agent<a class="anchor-link" href="#Implement-a-Basic-Driving-Agent">&#182;</a></h2><p>The first step to creating an optimized Q-Learning driving agent is getting the agent to actually take valid actions. In this case, a valid action is one of <code>None</code>, (do nothing) <code>'left'</code> (turn left), <code>right'</code> (turn right), or <code>'forward'</code> (go forward). For your first implementation, navigate to the <code>'choose_action()'</code> agent function and make the driving agent randomly choose one of these actions. Note that you have access to several class variables that will help you write this functionality, such as <code>'self.learning'</code> and <code>'self.valid_actions'</code>. Once implemented, run the agent file and simulation briefly to confirm that your driving agent is taking a random action each time step.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Basic-Agent-Simulation-Results">Basic Agent Simulation Results<a class="anchor-link" href="#Basic-Agent-Simulation-Results">&#182;</a></h3><p>To obtain results from the initial simulation, you will need to adjust following flags:</p>
<ul>
<li><code>'enforce_deadline'</code> - Set this to <code>True</code> to force the driving agent to capture whether it reaches the destination in time.</li>
<li><code>'update_delay'</code> - Set this to a small value (such as <code>0.01</code>) to reduce the time between steps in each trial.</li>
<li><code>'log_metrics'</code> - Set this to <code>True</code> to log the simluation results as a <code>.csv</code> file in <code>/logs/</code>.</li>
<li><code>'n_test'</code> - Set this to <code>'10'</code> to perform 10 testing trials.</li>
</ul>
<p>Optionally, you may disable to the visual simulation (which can make the trials go faster) by setting the <code>'display'</code> flag to <code>False</code>. Flags that have been set here should be returned to their default setting when debugging. It is important that you understand what each flag does and how it affects the simulation!</p>
<p>Once you have successfully completed the initial simulation (there should have been 20 training trials and 10 testing trials), run the code cell below to visualize the results. Note that log files are overwritten when identical simulations are run, so be careful with what log file is being loaded!
Run the agent.py file after setting the flags from projects/smartcab folder instead of projects/smartcab/smartcab.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[4]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span></span><span class="c1"># Load the &#39;sim_no-learning&#39; log file from the initial simulation results</span>
<span class="n">vs</span><span class="o">.</span><span class="n">plot_trials</span><span class="p">(</span><span class="s1">&#39;sim_no-learning.csv&#39;</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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IteLyFYROSciVrVujDHGCljGmPyrVq1a0GZpVapU8dauZK/hioyM9E6Ge/z4cT755JOA/SMiIkp9f6Lq1auzZcsWbwFx5cqVNGrUyBseHR3NjBkzzvs4WVlZfssxMTEsWrQIcAp5DRo04K233iImJgaAzz//HCCg4FoQ2QtYUVFRPPfcc4WOrxT7HogTkQdEZJrndZ5xbgFGA2vPP3nGGGPKAytgGWPO2z/+8Q9SUlJYt24dPXr08AsTEe68806mTZvGl19+GTAvWVkybNgwPvjgAwBiY2O9hRyABQsWeJtATpgwgalTp9K7d29atGjBO++8AzijAN5333106tSJzp07s3jxYgDi4uIYOHAgN910U0AzycGDB7N9+3bvhN0nT55k1apV3mH0a9SoQUpKClu2bOH2228PiNtXUlISffv2pVu3bnTr1s1bOJsxYwbr1q2jS5cuzJ8/n7i4OG/N3JEjRxg5ciQRERH06tWLxMREAObOncvEiRMZMGAALVq0KCsFsh+BlUAlIMznVWiquk1VdxRB2owxxpQTNsiFMaZIVKxY0W9IdV9333130R5s1YDAdU1ugDZ3QOZJiBseGN5igvM6lQLrr/MPGxyXr8OOHTuWefPmMWLECBITE5k4cSLr1q0Luu3BgwdZv34927dvJzo6muuuu46lS5eSkJDA5s2bSUlJoUePHvTr1w+ADRs2sGXLFpo3b+4XT2hoKKNHj+att97i7rvvZvny5QwcONBvAuIffviBTz/9lK+//pqPP/6Y0NBQv7g96tWrx8qVK6lSpQq7du0iJiaG+Ph4nnjiCZ566inef/99wCnwecyZM4euXbvy7rvvsnr1asaNG0dCQgIA27dv59NPPyU9PZ22bdty++23+81TVtqo6sMAIhLmLOrxEk6SMcaYcshqsIwxJp8iIiJISkoiNjY2YALs7EaOHElISAgdOnTwjv63fv16YmJiCA0NpX79+vTv35+NGzcC0LNnz4DClYdvM8FFixb51ZyBU4uVkJDAiBEjqF+/fkDcHmfPnuXWW2+lc+fOXH/99Xz33Xd5nvP69eu9fc8GDRpEamoqaWlON6arr76aypUrEx4eTr169bznWVqJSCcR+QanWd9WEdkkIjkPWfrrfqtEZEuQ17UFPP5tIhIvIvGHDx8u7GkYY4wp5awGyxhT9uRW41ShWu7hVcLz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DBgQuO6GG+COO+DkSRg+PDB8wgTnlZIC113nHxYXl6/Djh07lnnz5jFixAgSExOZOHEi69atC7rtwYMHWb9+Pdu3byc6OprrrruOpUuXkpCQwObNm0lJSaFHjx706+eMsbBhwwa2bNlC8+bNA+L67LPPaN68OS1btmTAgAGsWLGC0aNHs3XrVh599FE+++wzwsPDvc3xpk6dSv/+/Vm2bBlZWVkcP37cL75ly5axY8cOvv32Ww4dOkSHDh2YOHEiZ8+e5a677uK9996jbt26LF68mJkzZ/LKK68AToFow4YNrFixgocffphVq1Yxb9484uPjef7553O9dsGaBh46dIisrCxOnjzJjz/+SKdOnfL+EM7PSndgi8XACc9KVT2S8y7GGGNMwVgByxhj8ikiIoKkpCRiY2MZHqwQ52PkyJGEhITQoUMHDh06BMD69euJiYkhNDSU+vXr079/fzZu3MhFF11Ez549gxauwKktGzt2LOAU8l5//XVGjx7N6tWrue666wgPDwfg4osvBmD16tW89tprAISGhlKzZk2/+NauXetNR8OGDRk0aBAAO3bsYMuWLQwZMgRwmiv6Drs+evRoALp3705SUlK+r1tORAQRQVVp2LDhb9E/a6L7906fdQq0KO4DG2OMuXBYAcsYU/bkVuNUrVru4eHh+a6xCiY6Oprp06cTFxdHampqjttVrlzZ+97T9C23JnDVq1cPuj4rK4slS5awfPlyHn30UVSV1NRU0tPTz2t+qWD7qSodO3bkiy++CLqP55xCQ0PJzMws1HF9NWzYkPDwcFJSUryFQ18vv/xyjgNzFIaqBi/BGmOMMUXI+mAZY0wBTJw4kdmzZwftK5WXfv36sXjxYrKysjh8+DBr166lZ8+eue6zatUqIiMj2bdvH0lJSfzwww+MGTOGd999lyuuuIK33nrLW9DzNBG84oor+Mc//gE4BbRjx44FpGPRokVkZWVx8OBBPv30UwDatm3L4cOHvQWss2fPsnXr1lzTFxYWRnp6eoGvhUelSpWC1l59//33TJ48uUibDYpINRGZJSIvucutRWREkR3AGGOMwQpYxhhTII0bN+buu+8u1L6jRo3yDkgxaNAgnnzySS655JJc94mNjWXUqFF+68aMGcObb75Jx44dmTlzJv379ycyMpJp06YB8Oyzz/Lpp5/SuXNnunfvHlBI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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Question-3">Question 3<a class="anchor-link" href="#Question-3">&#182;</a></h3><p>Using the visualization above that was produced from your initial simulation, provide an analysis and make several observations about the driving agent. Be sure that you are making at least one observation about each panel present in the visualization. Some things you could consider:</p>
<ul>
<li><em>How frequently is the driving agent making bad decisions? How many of those bad decisions cause accidents?</em></li>
<li><em>Given that the agent is driving randomly, does the rate of reliability make sense?</em></li>
<li><em>What kind of rewards is the agent receiving for its actions? Do the rewards suggest it has been penalized heavily?</em></li>
<li><em>As the number of trials increases, does the outcome of results change significantly?</em></li>
<li><em>Would this Smartcab be considered safe and/or reliable for its passengers? Why or why not?</em></li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><strong>Answer:</strong></p>
<ul>
<li>As per the above visualization, the driving agent is making bad decisions around ~41% of the time and around ~4% to ~8% of the bad descisions cause minor &amp; major accidents</li>
<li>By looking at the Trial Rolling Rate of Relibility chart it seems that the chart makes perfect sense because the line remains relatively under 20% - 10% and this is expected as the actions of agent are completely random as it has not done any learning. </li>
<li>The agent is recieving appropriate rewards for its actions as the penalty is going down from -5 to -4 which clearly shows an improvment in performance. Hence, we can say that the rewards are not been penalized heavily.</li>
<li>As the number of trials increases the outcome of the results doesnot change significantly. Every chart is showing a consistent result with a little variation only. Regardless of the increase in number of trials the agents actions are random with no learning or change in behaviour. The final output states that the Agent has recieved F in safety as well as in Reliability. </li>
<li>As per my observations, the smart cab can not be considered safe and/or reliable for its passengers because of the below reasons- <ul>
<li>The agent takes bad descisions ~41 % of the time hence would not be able to take passengers to their destination.</li>
<li>Agents random actions lead to both major and minor accidents and traffic violations. </li>
<li>Performnce of the cab did not improve even after 20 trials. </li>
<li>Rating recieved in safety and reliability is F which can not be considered good. </li>
</ul>
</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<hr>
<h2 id="Inform-the-Driving-Agent">Inform the Driving Agent<a class="anchor-link" href="#Inform-the-Driving-Agent">&#182;</a></h2><p>The second step to creating an optimized Q-learning driving agent is defining a set of states that the agent can occupy in the environment. Depending on the input, sensory data, and additional variables available to the driving agent, a set of states can be defined for the agent so that it can eventually <em>learn</em> what action it should take when occupying a state. The condition of <code>'if state then action'</code> for each state is called a <strong>policy</strong>, and is ultimately what the driving agent is expected to learn. Without defining states, the driving agent would never understand which action is most optimal -- or even what environmental variables and conditions it cares about!</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Identify-States">Identify States<a class="anchor-link" href="#Identify-States">&#182;</a></h3><p>Inspecting the <code>'build_state()'</code> agent function shows that the driving agent is given the following data from the environment:</p>
<ul>
<li><code>'waypoint'</code>, which is the direction the <em>Smartcab</em> should drive leading to the destination, relative to the <em>Smartcab</em>'s heading.</li>
<li><code>'inputs'</code>, which is the sensor data from the <em>Smartcab</em>. It includes <ul>
<li><code>'light'</code>, the color of the light.</li>
<li><code>'left'</code>, the intended direction of travel for a vehicle to the <em>Smartcab</em>'s left. Returns <code>None</code> if no vehicle is present.</li>
<li><code>'right'</code>, the intended direction of travel for a vehicle to the <em>Smartcab</em>'s right. Returns <code>None</code> if no vehicle is present.</li>
<li><code>'oncoming'</code>, the intended direction of travel for a vehicle across the intersection from the <em>Smartcab</em>. Returns <code>None</code> if no vehicle is present.</li>
</ul>
</li>
<li><code>'deadline'</code>, which is the number of actions remaining for the <em>Smartcab</em> to reach the destination before running out of time.</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Question-4">Question 4<a class="anchor-link" href="#Question-4">&#182;</a></h3><p><em>Which features available to the agent are most relevant for learning both <strong>safety</strong> and <strong>efficiency</strong>? Why are these features appropriate for modeling the </em>Smartcab<em> in the environment? If you did not choose some features, why are those features</em> not <em>appropriate? Please note that whatever features you eventually choose for your agent's state, must be argued for here. That is: your code in agent.py should reflect the features chosen in this answer.</em></p>
<p>NOTE: You are not allowed to engineer new features for the smartcab.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><strong>Answer:</strong></p>
<p>Below features can be considered as the most relevant for learning both safety and efficiency -</p>
<p><strong>Safety:</strong></p>
<ul>
<li>light - The light state is critical for safety so that a vehicle should know when it can move or not. In particular, a vehicle must stop at a red light and move at a green light to ensure safety of itself as well as every other vehicle present on road. Following the base rule of traffic light can prevent collisions on road. </li>
<li>left - The direction of travel is most important to determine whether it's safe to proceed or not.</li>
<li>oncoming - The Smartcab must know if there is a vehicle coming from the opposite direction when it is trying to make a left turn. If the agent decides to drive into oncoming traffic, then it will cause either a traffic violation or, if there is a vehicle present, an accident.</li>
</ul>
<p><strong>Efficiency</strong></p>
<ul>
<li>waypoint - The waypoint is most appropriate for achieving efficiency as this allows the agent to know where it can go because without knowing the path the Agent might never reach its intended destination. This will ensure the smartcab reaches the destination in the most efficient manner possible.</li>
</ul>
<p>I would consider the below feature not as relevant for the following reasons:</p>
<ul>
<li>right - The input right rule is not essential for the car to know, since it does not play a role in the rules of the grid world traffic and is not very essential for efficiency.</li>
<li>deadline - Though meeting the deadline is important but in order to meet deadline there are many factors that can be compromised on road like ignoring other vehicles and traffic lights, which would compromise safety and may result in accidents.  </li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Define-a-State-Space">Define a State Space<a class="anchor-link" href="#Define-a-State-Space">&#182;</a></h3><p>When defining a set of states that the agent can occupy, it is necessary to consider the <em>size</em> of the state space. That is to say, if you expect the driving agent to learn a <strong>policy</strong> for each state, you would need to have an optimal action for <em>every</em> state the agent can occupy. If the number of all possible states is very large, it might be the case that the driving agent never learns what to do in some states, which can lead to uninformed decisions. For example, consider a case where the following features are used to define the state of the <em>Smartcab</em>:</p>
<p><code>('is_raining', 'is_foggy', 'is_red_light', 'turn_left', 'no_traffic', 'previous_turn_left', 'time_of_day')</code>.</p>
<p>How frequently would the agent occupy a state like <code>(False, True, True, True, False, False, '3AM')</code>? Without a near-infinite amount of time for training, it's doubtful the agent would ever learn the proper action!</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Question-5">Question 5<a class="anchor-link" href="#Question-5">&#182;</a></h3><p><em>If a state is defined using the features you've selected from <strong>Question 4</strong>, what would be the size of the state space? Given what you know about the environment and how it is simulated, do you think the driving agent could learn a policy for each possible state within a reasonable number of training trials?</em><br>
<strong>Hint:</strong> Consider the <em>combinations</em> of features to calculate the total number of states!</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><strong>Answer:</strong>
To know whether the driving could learn a policy or not for each possible state within a reasonable number of trials first, we must consider each feature and the number of states each one has:</p>
<ul>
<li>waypoint - [left, right, forward]  : 3</li>
<li>inputs-light - [red, green] : 2</li>
<li>inputs-left - [left, right, forward, None] : 4</li>
<li>inputs-oncoming - [left, right, forward, None] : 4</li>
</ul>
<p>The possible combinations based on just the features are 3x2x4x4 or 96 total number of states but, if I also add the possible actions which can be - [left, right, forward, None] : 4
then it is 3x2x4x4x4 or 384 possible combinations.</p>
<p>Since, 384 is not a large number, so I think that the driving agent could learn a policy for each possible state within a reasonable number of training trials.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Update-the-Driving-Agent-State">Update the Driving Agent State<a class="anchor-link" href="#Update-the-Driving-Agent-State">&#182;</a></h3><p>For your second implementation, navigate to the <code>'build_state()'</code> agent function. With the justification you've provided in <strong>Question 4</strong>, you will now set the <code>'state'</code> variable to a tuple of all the features necessary for Q-Learning. Confirm your driving agent is updating its state by running the agent file and simulation briefly and note whether the state is displaying. If the visual simulation is used, confirm that the updated state corresponds with what is seen in the simulation.</p>
<p><strong>Note:</strong> Remember to reset simulation flags to their default setting when making this observation!</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<hr>
<h2 id="Implement-a-Q-Learning-Driving-Agent">Implement a Q-Learning Driving Agent<a class="anchor-link" href="#Implement-a-Q-Learning-Driving-Agent">&#182;</a></h2><p>The third step to creating an optimized Q-Learning agent is to begin implementing the functionality of Q-Learning itself. The concept of Q-Learning is fairly straightforward: For every state the agent visits, create an entry in the Q-table for all state-action pairs available. Then, when the agent encounters a state and performs an action, update the Q-value associated with that state-action pair based on the reward received and the iterative update rule implemented. Of course, additional benefits come from Q-Learning, such that we can have the agent choose the <em>best</em> action for each state based on the Q-values of each state-action pair possible. For this project, you will be implementing a <em>decaying,</em> $\epsilon$<em>-greedy</em> Q-learning algorithm with <em>no</em> discount factor. Follow the implementation instructions under each <strong>TODO</strong> in the agent functions.</p>
<p>Note that the agent attribute <code>self.Q</code> is a dictionary: This is how the Q-table will be formed. Each state will be a key of the <code>self.Q</code> dictionary, and each value will then be another dictionary that holds the <em>action</em> and <em>Q-value</em>. Here is an example:</p>

<pre><code>{ 'state-1': { 
    'action-1' : Qvalue-1,
    'action-2' : Qvalue-2,
     ...
   },
  'state-2': {
    'action-1' : Qvalue-1,
     ...
   },
   ...
}</code></pre>
<p>Furthermore, note that you are expected to use a <em>decaying</em> $\epsilon$ <em>(exploration) factor</em>. Hence, as the number of trials increases, $\epsilon$ should decrease towards 0. This is because the agent is expected to learn from its behavior and begin acting on its learned behavior. Additionally, The agent will be tested on what it has learned after $\epsilon$ has passed a certain threshold (the default threshold is 0.05). For the initial Q-Learning implementation, you will be implementing a linear decaying function for $\epsilon$.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Q-Learning-Simulation-Results">Q-Learning Simulation Results<a class="anchor-link" href="#Q-Learning-Simulation-Results">&#182;</a></h3><p>To obtain results from the initial Q-Learning implementation, you will need to adjust the following flags and setup:</p>
<ul>
<li><code>'enforce_deadline'</code> - Set this to <code>True</code> to force the driving agent to capture whether it reaches the destination in time.</li>
<li><code>'update_delay'</code> - Set this to a small value (such as <code>0.01</code>) to reduce the time between steps in each trial.</li>
<li><code>'log_metrics'</code> - Set this to <code>True</code> to log the simluation results as a <code>.csv</code> file and the Q-table as a <code>.txt</code> file in <code>/logs/</code>.</li>
<li><code>'n_test'</code> - Set this to <code>'10'</code> to perform 10 testing trials.</li>
<li><code>'learning'</code> - Set this to <code>'True'</code> to tell the driving agent to use your Q-Learning implementation.</li>
</ul>
<p>In addition, use the following decay function for $\epsilon$:</p>
<p>$$ \epsilon_{t+1} = \epsilon_{t} - 0.05, \hspace{10px}\textrm{for trial number } t$$</p>
<p>If you have difficulty getting your implementation to work, try setting the <code>'verbose'</code> flag to <code>True</code> to help debug. Flags that have been set here should be returned to their default setting when debugging. It is important that you understand what each flag does and how it affects the simulation!</p>
<p>Once you have successfully completed the initial Q-Learning simulation, run the code cell below to visualize the results. Note that log files are overwritten when identical simulations are run, so be careful with what log file is being loaded!</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[22]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span></span><span class="c1"># Load the &#39;sim_default-learning&#39; file from the default Q-Learning simulation</span>
<span class="n">vs</span><span class="o">.</span><span class="n">plot_trials</span><span class="p">(</span><span class="s1">&#39;sim_default-learning.csv&#39;</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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pW7dur4O52zkdcTc9BFsS5UqdX4iM8YY4xOF9qDhC4GNImhM0bZlyxYaNGhglauLnKqydetWGjZsmGG+iKxV1TAfhZUnIjIIuE5V/8+dvgNopaoPZbeOlT3GGFN0FUTZU5iDXBR5qpqlOdUYU7RY5erid4F/xvkdMdcYY8xF7pKuYP3++++0bduWOXPm+DoUY4wxF6ZcR8w1xhhzabmkK1hHjhzh5MmTDBgwgLVr1/o6HGNMERMXF0doaCihoaFUrVqV6tWrp0+fPn06y/KHDx/mvffeyzXf5ORkLrvsMq/z/fz80rfRokULVq9ena+Yx40bl37TsjdNmjTxejNwZjt37mT69Onp0z/88AOPPvpovmK5FKhqMpA2Yu4W4DNV3eTbqIwxxvjSJT3IRalSpTh16hT33XcfzZs393U4xpgiplKlSundiCdMmEBAQED6iEjepFWwRowYcdbbDAwMTN/mggULGDt2bJaRpc7Whg0bKF68OEuXLuXEiROUKVMm22XTKliDBw8GoHXr1rRunWXsBoP3EXONMcZcui7pFqwGDRowduxY3nzzzQv9HgBjzHn20ksv0aRJE5o0acJbb70FwJgxY9i2bRuhoaGMGTOGhIQEunXrRvPmzQkODs4yRG9uEhISqFChQvr77PKaNGkS11xzDddeey3bt2/PNr/IyEiGDBlCt27dMqz/66+/0q1bN0JCQmjevDkxMTGMGTOGZcuWERoayptvvsnixYvp168fAIcOHSI8PJzg4GDatWvHxo0bAaf17K677qJz587Uq1ePd955B4DExER69+5NSEgITZo0YebMmfk6DsYYY8wFRVUv2VeLFi3Um9TUVD127JjXNGPM+bN58+YM088884wCCugzzzyTZflRo0alp7/yyitZ0u++++709Pfffz9fsTzzzDP68ssvq6rqDz/8oMHBwXr8+HFNSEjQBg0a6Pr163X79u0aEhKSvs7p06c1ISFBVVX379+vV111laqqnjlzRsuXL59lG2fOnNFixYppSEiIXnPNNVq+fHn96aefcswrLZakpCQ9evSo1qlTR19//XWv+1CvXj2NjY3VBQsWaP/+/dPnN2/eXOfNm6eqqidOnNDjx4/rokWL9MYbb0xfxnN6xIgR+uyzz6qq6v/+9z9N+y0dO3asdujQQU+dOqX79+/XihUranJysk6fPl1H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cd5XAUO996cA74qIaFFe6Cs3iR/U6g/VroPYEbDyNWfx5O3Tod7D0OgZKBaa/XmMMdkaMGAAFSpU4NNPP6Vv377p2idPnswjjzxC3759ufPOO2nWrJkLURqT3h13ELF8OcE5ec7GjUn45BO2nu1x+/bt82/VqlWDqVOnrm3WrFliz549a3bu3Pnw448/vjc4OLhFv3794ubMmVMqNDQ05euvv95QtWrV5LTHT506tdSgQYMiUlJSaNasWcKECRM2lyhRQi+44IImN954495Zs2aVvueee/YcPnzYf+zYsRWSkpKkRo0aiVOmTNk4d+7cEr/++mvY3LlzS7366qtVvv766/VDhgyp0qNHj0O33377gazOff311++bOXNmaHJyskyaNGlDixYtjqeNq0uXLpH79+8PrF+/fsO33npry4oVK4LOvH6pUqU8W7duDbjjjjuqb9mypTjAu+++u/ntt9+utHXr1uL169dv2KlTp/gPPvhg23333Rf++++/h4qIPvnkkzvvvvvuAzNmzCj1f//3f1UqVqyYFBsbG7x+/XpfPwtm646pd0Qs37M8Z39HKjZO+OSqT876d2THjh0Bt99+e/Xt27cXA3jzzTe3XHbZZUdnzZoV/Nhjj1U7fvy4X1BQkGfcuHEbmzVrlvjOO++U+/HHH0MTExP9EhIS/J599tmdL774YtWyZcsmrV69ukSTJk0Svvvuu41+fn60adOm3uuvv761Y8eOCcHBwS3uvPPOPT///HNoUFCQZ8aMGesiIiKSV6xYUfymm26qmZKSIl26dDk0evToSgkJCYvSxnjTTTdV27ZtW/FevXrV6dev396OHTseySi25ORkBg4cGP7HH3+UBujfv/9eVWXPnj2BnTp1iixTpkzyvHnz1nz44Ydl33jjjcqqKl26dDn4wQcfbAenh2/AgAG7f//999IjRozY1q1btyM58bMpKrLtIlTVS4DOQBwwWkSWicizPpz7AjjtD+A27zZfBYlItIjMFZGr0zaIyFhgF1AfGHnm9VQ1GWcoYz5atbeQCigJTYdCzzVOhUHPCVg5AqbXgbUfOJUIjTHnpWTJktx8883MnDmT22+/PV37Z599RlxcHCNHjmT69OkuRGhM/pKYmOiXdojgRx99VKZcuXIp//vf/7b079+/5ujRo8scPHgw4PHHH98LcOzYMb+WLVsmxMbG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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Question-6">Question 6<a class="anchor-link" href="#Question-6">&#182;</a></h3><p>Using the visualization above that was produced from your default Q-Learning simulation, provide an analysis and make observations about the driving agent like in <strong>Question 3</strong>. Note that the simulation should have also produced the Q-table in a text file which can help you make observations about the agent's learning. Some additional things you could consider:</p>
<ul>
<li><em>Are there any observations that are similar between the basic driving agent and the default Q-Learning agent?</em></li>
<li><em>Approximately how many training trials did the driving agent require before testing? Does that number make sense given the epsilon-tolerance?</em></li>
<li><em>Is the decaying function you implemented for $\epsilon$ (the exploration factor) accurately represented in the parameters panel?</em></li>
<li><em>As the number of training trials increased, did the number of bad actions decrease? Did the average reward increase?</em></li>
<li><em>How does the safety and reliability rating compare to the initial driving agent?</em></li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><strong>Answer:</strong></p>
<ul>
<li><p>Compairing basic driving agent and the default Q-learning agent I come to an observation that all results which includes bad actions, violations, accidents, rate of reliability, rewards per action are not at all same rather they have all dramatically went down in case of Q-Learning agent. Though the safety and reliability rating are still poor which is F but the scores are certainly improved by the end of trials.</p>
</li>
<li><p>Approximately driving agent require 20 trials before testing. As we can see in the 'Parameter Value' graph that the epsilon is represented accurately and it decreases by 0.05 every time, which is consistent with the function, 1/0.05 = 20, and this is consistent with the number of trials required.</p>
</li>
<li><p>Yes, the decaying function I have imlemented for the exploration factor is accurately represented in parameters panel because it is steadily decreasing with each trial across 20 trials. In 20 trials, epsilon is decaying from 1 to 0.</p>
</li>
<li><p>Yes as the number of training trials increased the number of bad actions gradually decrease as it is clearly shown in the graph by the end of 20 trials the frequency of bad actions goes down from 34% to 15 %. Also, the average reward increased from -4 to -1.</p>
</li>
<li><p>The safety rating  and realiabilty rating are still the same which is F even though the new Q-Learning agent performance has improved compare to the basic driving agent.</p>
</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<hr>
<h2 id="Improve-the-Q-Learning-Driving-Agent">Improve the Q-Learning Driving Agent<a class="anchor-link" href="#Improve-the-Q-Learning-Driving-Agent">&#182;</a></h2><p>The third step to creating an optimized Q-Learning agent is to perform the optimization! Now that the Q-Learning algorithm is implemented and the driving agent is successfully learning, it's necessary to tune settings and adjust learning paramaters so the driving agent learns both <strong>safety</strong> and <strong>efficiency</strong>. Typically this step will require a lot of trial and error, as some settings will invariably make the learning worse. One thing to keep in mind is the act of learning itself and the time that this takes: In theory, we could allow the agent to learn for an incredibly long amount of time; however, another goal of Q-Learning is to <em>transition from experimenting with unlearned behavior to acting on learned behavior</em>. For example, always allowing the agent to perform a random action during training (if $\epsilon = 1$ and never decays) will certainly make it <em>learn</em>, but never let it <em>act</em>. When improving on your Q-Learning implementation, consider the implications it creates and whether it is logistically sensible to make a particular adjustment.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Improved-Q-Learning-Simulation-Results">Improved Q-Learning Simulation Results<a class="anchor-link" href="#Improved-Q-Learning-Simulation-Results">&#182;</a></h3><p>To obtain results from the initial Q-Learning implementation, you will need to adjust the following flags and setup:</p>
<ul>
<li><code>'enforce_deadline'</code> - Set this to <code>True</code> to force the driving agent to capture whether it reaches the destination in time.</li>
<li><code>'update_delay'</code> - Set this to a small value (such as <code>0.01</code>) to reduce the time between steps in each trial.</li>
<li><code>'log_metrics'</code> - Set this to <code>True</code> to log the simluation results as a <code>.csv</code> file and the Q-table as a <code>.txt</code> file in <code>/logs/</code>.</li>
<li><code>'learning'</code> - Set this to <code>'True'</code> to tell the driving agent to use your Q-Learning implementation.</li>
<li><code>'optimized'</code> - Set this to <code>'True'</code> to tell the driving agent you are performing an optimized version of the Q-Learning implementation.</li>
</ul>
<p>Additional flags that can be adjusted as part of optimizing the Q-Learning agent:</p>
<ul>
<li><code>'n_test'</code> - Set this to some positive number (previously 10) to perform that many testing trials.</li>
<li><code>'alpha'</code> - Set this to a real number between 0 - 1 to adjust the learning rate of the Q-Learning algorithm.</li>
<li><code>'epsilon'</code> - Set this to a real number between 0 - 1 to adjust the starting exploration factor of the Q-Learning algorithm.</li>
<li><code>'tolerance'</code> - set this to some small value larger than 0 (default was 0.05) to set the epsilon threshold for testing.</li>
</ul>
<p>Furthermore, use a decaying function of your choice for $\epsilon$ (the exploration factor). Note that whichever function you use, it <strong>must decay to </strong><code>'tolerance'</code><strong> at a reasonable rate</strong>. The Q-Learning agent will not begin testing until this occurs. Some example decaying functions (for $t$, the number of trials):</p>
<p>$$ \epsilon = a^t, \textrm{for } 0 &lt; a &lt; 1 \hspace{50px}\epsilon = \frac{1}{t^2}\hspace{50px}\epsilon = e^{-at}, \textrm{for } 0 &lt; a &lt; 1 \hspace{50px} \epsilon = \cos(at), \textrm{for } 0 &lt; a &lt; 1$$
You may also use a decaying function for $\alpha$ (the learning rate) if you so choose, however this is typically less common. If you do so, be sure that it adheres to the inequality $0 \leq \alpha \leq 1$.</p>
<p>If you have difficulty getting your implementation to work, try setting the <code>'verbose'</code> flag to <code>True</code> to help debug. Flags that have been set here should be returned to their default setting when debugging. It is important that you understand what each flag does and how it affects the simulation!</p>
<p>Once you have successfully completed the improved Q-Learning simulation, run the code cell below to visualize the results. Note that log files are overwritten when identical simulations are run, so be careful with what log file is being loaded!</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[24]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython2"><pre><span></span><span class="c1"># Load the &#39;sim_improved-learning&#39; file from the improved Q-Learning simulation</span>
<span class="n">vs</span><span class="o">.</span><span class="n">plot_trials</span><span class="p">(</span><span class="s1">&#39;sim_improved-learning.csv&#39;</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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PffcY6336quvWssbNWr0j665Y8cOp9fbt2+fOnXqlF3dS5cuqYsXL6rk5GQ1efJka93t27errl27Wre///57u+Nefvll674pU6YopZRq3bq1tWz9+vX5ttO2bXFxcf/onjVNK1zADnUb/N/QD/3QD/3QD/3I7+FqiKBt90zLGxDL3VlOLYKqt/8HKLnnWP3f//0fmzZtIiQkhLvuustabrv2lLM5UrbOnTtHTk4OXl5ehISEOCS68PX1dTjmySefdLpY8eOPP87GjRsdyrdu3WrXJttEHQDdunUjIiKC1NRUa29bbGysdf+mTZto166dy/vw8fGxLnRsm91Q0zRN0zRN066Xq3WwnC9cVBylxjmW+Yff/HZcBx8fH7vA5t133+W9997jtddes1v76b///S9Vq1alZMmS1mF2eXnooYeoUKECZcuWZf/+/Q77Q0ND6dy5s3W7cePGPPjggw710tPTnQZXYArIqlSpQlRUFFWqVHFIL1+1alWqVKlCzZo1rXPC/vWvf1n355d2XSllDa4A3n//fZf1NU3TNE3TNM0drnqwaovIPkw9WTXMzzFvK6VUg0Jv3e1iSw/HssCCLP9w65QsWZK5c+dak1nY9grZCg0N5dixY2RmZuY5b8siv3WwKlWq5HQBYos+ffrw888/c+7cOZfXmTUr76XXNm3axNNPPw3AU089xcKFC+3W+8ovYYWIMGHCBEaOHAk4JtHQNE3TNE3TtOvhKsCqc9Nacbu7EuNYpvLPpHe7sB1et3v3bg4cOOB0MWFPT888g6uXXnqJS5cukZOTg4eHB+XKlcNoNOab8MLWli1bePvtt/PtIQN45JFHWLRoEffffz/p6enUqFGDHTuuLc3h6Xktk+O3337Lfffdx8SJE/noo4/w9va2258X2x6s3377jSNHjhAZGen2/WiapmmapmlabnkGWEqpUzezIbc3J9kCc4pGSu/169czbpx9Isjly5eTmJhI69atnc6XcuaHH34gMTERgDNnzlCxYkW323D+/HlatmzJ0aNH86zz+uuv07ZtWx566CEA9u7dS3JysvWaly5dsqufO+PfTz/9xMCBA91uE5h60vbt28d3333Htm3bmD17Nh9++GGBzqFpmqZpmqZpttxZB0sTJ1PVlMGx7DZ05coVfv31V7uy0aNHA/Dyyy/zySefuHWegq6DtWfPHmbN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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Question-7">Question 7<a class="anchor-link" href="#Question-7">&#182;</a></h3><p>Using the visualization above that was produced from your improved Q-Learning simulation, provide a final analysis and make observations about the improved driving agent like in <strong>Question 6</strong>. Questions you should answer:</p>
<ul>
<li><em>What decaying function was used for epsilon (the exploration factor)?</em></li>
<li><em>Approximately how many training trials were needed for your agent before begining testing?</em></li>
<li><em>What epsilon-tolerance and alpha (learning rate) did you use? Why did you use them?</em></li>
<li><em>How much improvement was made with this Q-Learner when compared to the default Q-Learner from the previous section?</em></li>
<li><em>Would you say that the Q-Learner results show that your driving agent successfully learned an appropriate policy?</em></li>
<li><em>Are you satisfied with the safety and reliability ratings of the </em>Smartcab<em>?</em></li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><strong>Answer:</strong></p>
<ul>
<li>An epsilon = e^(-at) decay function was used, with epsilon starting at 1.00. This was picked because it is important to have a great wealth of learning early on, with a gradual decline into exploration.</li>
<li>Approximately 1200 trials were needed before testing was completed.</li>
<li>I have used an epsilon tolerance of 0.01 and an alpha of 0.002.  I have run ~1200 trials using the very low alpha to allow the model sufficient trials for learning .  A large number of trials are important to increase the safety rating to maximum. As a result of the small alpha, a smaller tolerance is more appropriate - otherwise a large proportion of trials would be missed towards the end of the decay.</li>
<li>A drastic improvement can be seen in this Q-Learner compared to the default Q-Learner from the previous section. The Safety Rating has increased from <strong>F</strong> to <strong>A+</strong>. Also, the Reliability Rating has increased from <strong>F</strong> to <strong>A</strong>. Getting such ratings would definitely make Smartcab safe for deployment.</li>
<li>Yes, I would definitely say that the Driving agent has succesfully learned an appropriate policy as the ratings have improved drastically and so the smartcab's performance.</li>
<li>Yes, I am satisfied with safety and reliability ratings of Smartcab. But as, learning is an ongoing process so, there is always a scope of learning. </li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Define-an-Optimal-Policy">Define an Optimal Policy<a class="anchor-link" href="#Define-an-Optimal-Policy">&#182;</a></h3><p>Sometimes, the answer to the important question <em>"what am I trying to get my agent to learn?"</em> only has a theoretical answer and cannot be concretely described. Here, however, you can concretely define what it is the agent is trying to learn, and that is the U.S. right-of-way traffic laws. Since these laws are known information, you can further define, for each state the <em>Smartcab</em> is occupying, the optimal action for the driving agent based on these laws. In that case, we call the set of optimal state-action pairs an <strong>optimal policy</strong>. Hence, unlike some theoretical answers, it is clear whether the agent is acting "incorrectly" not only by the reward (penalty) it receives, but also by pure observation. If the agent drives through a red light, we both see it receive a negative reward but also know that it is not the correct behavior. This can be used to your advantage for verifying whether the <strong>policy</strong> your driving agent has learned is the correct one, or if it is a <strong>suboptimal policy</strong>.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Question-8">Question 8<a class="anchor-link" href="#Question-8">&#182;</a></h3><ol>
<li><p>Please summarize what the optimal policy is for the smartcab in the given environment. What would be the best set of instructions possible given what we know about the environment? 
<em>You can explain with words or a table, but you should thoroughly discuss the optimal policy.</em></p>
</li>
<li><p>Next, investigate the <code>'sim_improved-learning.txt'</code> text file to see the results of your improved Q-Learning algorithm. <em>For each state that has been recorded from the simulation, is the <strong>policy</strong> (the action with the highest value) correct for the given state? Are there any states where the policy is different than what would be expected from an optimal policy?</em></p>
</li>
<li><p>Provide a few examples from your recorded Q-table which demonstrate that your smartcab learned the optimal policy. Explain why these entries demonstrate the optimal policy.</p>
</li>
<li><p>Try to find at least one entry where the smartcab did <em>not</em> learn the optimal policy.  Discuss why your cab may have not learned the correct policy for the given state.</p>
</li>
</ol>
<p>Be sure to document your <code>state</code> dictionary below, it should be easy for the reader to understand what each state represents.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><strong>Answer:</strong></p>
<p>Based on the inputs I've discussed previously (which are waypoint,left,light,oncoming) an optimal policy would be to look at the environment given the state of above features and then Agent should make a safe, and reliable decision.</p>
<p>The decision made for the best action would be considered the optimal policy. For example. If on a red light their is a car turning left and a car turning right and the waypoint is None, then the Agent should remain idle in order to have optimal policy which will ensure safety as well as reliability.
Also, any movement in a red light state should have the highest penalty.</p>
<p>The state should look like this with the possible action of None, forward, left and right:</p>
<table>
<thead><tr>
<th style="text-align:center">N</th>
<th style="text-align:center">state</th>
<th style="text-align:center">actions</th>
<th>policy</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center">1</td>
<td style="text-align:center">{'forward', 'red', None, None}</td>
<td style="text-align:center">right</td>
<td>optimal</td>
</tr>
<tr>
<td style="text-align:center">2</td>
<td style="text-align:center">{'forward', 'red', None, None}</td>
<td style="text-align:center">right</td>
<td>incorrect</td>
</tr>
<tr>
<td style="text-align:center">3</td>
<td style="text-align:center">{'forward', 'red', None, None}</td>
<td style="text-align:center">right</td>
<td>incorrect</td>
</tr>
<tr>
<td style="text-align:center">4</td>
<td style="text-align:center">{'forward', 'red', None, None}</td>
<td style="text-align:center">right</td>
<td>suboptimal</td>
</tr>
</tbody>
</table>
<p>The best set of instructons to achieve optimal policy can be as below -</p>
<ul>
<li>Whereas, in green light state movement should be there , but certain conditions should be satisfied.</li>
<li>Also, if the oncoming traffic is in a direction which will cause a collision, the action should be avoided.</li>
<li>If the oncoming traffic is in the same direction as the waypoint, the waypoint direction should be given preference.</li>
<li>The smartcab should also learn the left turn rule, where it is not allowed to turn left if the oncoming traffic is turning right.</li>
</ul>
<p>The policy created by the learner displays the following states:</p>
<p><strong>Correct policy observation: Key: (waypoint, left traffic, light, oncoming traffic)</strong></p>
<p>('forward', 'forward', 'red', 'left')
 -- forward : -0.56
 -- right : -0.28
 -- None : 0.22
 -- left : -0.40
This is an optimal policy because cab is idle in red light state and it is getting a positive reward.</p>
<p>('forward', 'forward', 'green', 'forward')
 -- forward : 0.14
 -- right : 0.01
 -- None : -0.06
 -- left : -0.47
Since the waypoint is forward and the light is green so on moving forward or aking right the cab is getting a positive reward hence this is an opimal policy.</p>
<p><strong>Incorrect/unexpected policy observation:</strong></p>
<p>('left', 'left', 'green', 'None')
 -- forward : 0.05
 -- right : 0.29
 -- None : -0.28
 -- left : 0.09</p>
<p>We need to go left, and we can go left but surprisingly there are positive rewards associated with forward and right also on a green light which may mislead the driving agent in taking the right descision. Hence, it ia not an optimal policy. 
Here the cab may not have have learned the correct optimal policy because, it has learnt to move away from the waypoint rather than to wait till it's safe to follow the waypoint. It also shows safety on priority over reliability.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<hr>
<h3 id="Optional:-Future-Rewards---Discount-Factor,-'gamma'">Optional: Future Rewards - Discount Factor, <code>'gamma'</code><a class="anchor-link" href="#Optional:-Future-Rewards---Discount-Factor,-'gamma'">&#182;</a></h3><p>Curiously, as part of the Q-Learning algorithm, you were asked to <strong>not</strong> use the discount factor, <code>'gamma'</code> in the implementation. Including future rewards in the algorithm is used to aid in propagating positive rewards backwards from a future state to the current state. Essentially, if the driving agent is given the option to make several actions to arrive at different states, including future rewards will bias the agent towards states that could provide even more rewards. An example of this would be the driving agent moving towards a goal: With all actions and rewards equal, moving towards the goal would theoretically yield better rewards if there is an additional reward for reaching the goal. However, even though in this project, the driving agent is trying to reach a destination in the allotted time, including future rewards will not benefit the agent. In fact, if the agent were given many trials to learn, it could negatively affect Q-values!</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Optional-Question-9">Optional Question 9<a class="anchor-link" href="#Optional-Question-9">&#182;</a></h3><p><em>There are two characteristics about the project that invalidate the use of future rewards in the Q-Learning algorithm. One characteristic has to do with the </em>Smartcab<em> itself, and the other has to do with the environment. Can you figure out what they are and why future rewards won't work for this project?</em></p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><strong>Answer:</strong></p>
<p>The Smart Cab</p>
<ul>
<li>The traffic is constantly moving around the smart cab so, the decisions made by the agent in each state does not depend on previous or future positions. The agent does not know about the number of cars, traffic light, etc. at the next step, and therefore he lacks the opportunity to improve the results by planning the route as a whole in advance. At each step, the decision is made independently of all the others,so there is no point of future rewards. The destination changes with every trial, so the previous learnings can not be used across into different future trials, as each time Q values could be overfitted towards a particular start point and destination- which is irrelevant to the next trial. </li>
</ul>
<p>The Environment</p>
<ul>
<li>The environment kept on changing, let us assume sometimes it "is_raining', 'is_foggy' etc..so, in these situations previous learning can not be used and hence the future rewards can not be fixed. In addition, there are mulitple other agents that are making their own descisions and including them in your state space would make your MDP too large to handle realistically. Predicting Q-Learning based upon traffic of a location or enviornment chnges in advance will be different by the actual time of the day or by when the Smartcab reaches particular location.</li>
</ul>
<p>There is only one input state that the Smartcab can accurately calculate in future states - the waypoint. This would not provide sufficient input for determining future rewards.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<blockquote><p><strong>Note</strong>: Once you have completed all of the code implementations and successfully answered each question above, you may finalize your work by exporting the iPython Notebook as an HTML document. You can do this by using the menu above and navigating to<br>
<strong>File -&gt; Download as -&gt; HTML (.html)</strong>. Include the finished document along with this notebook as your submission.</p>
</blockquote>

</div>
</div>
</div>
    </div>
  </div>
</body>

 


</html>
