# MODULE-2-ASSIGNMENT

.in_progress,
.done {
  color: #C60;
  border: 1px solid;
  border-radius: 3px;
  padding: .1em 0.4em;
  font-weight: normal;
  margin-left: .2em;
  vertical-align: middle;
  font-size: 0.9em;
}
.done { color: #009933; }

@media print {
    body { color: #000; }
    .navbar, #intro, input[type="checkbox"], .done, .in_progress { display: none; }
    a { color: #000; text-decoration: underline; }
    a[href]:after { content: none !important; }
    .tab-content > .tab-pane, .pill-content > .pill-pane { display: block; }
    .tab-pane { page-break-after: always; }
}

ul {
  list-style-type: none;
  padding-left: 22px;
}
ul li ul {
  padding-top: 0;
}
h3 {
  margin-bottom: 0;
}
.checkbox label,
.radio label {
  padding-left: 24px;
}
.checkbox input[type=checkbox],
.checkbox-inline input[type=checkbox],
.radio input[type=radio],
.radio-inline input[type=radio] {
  margin-left: -24px;
}

.table_of_contents {
  margin-left: 0;
  padding: 0;
  line-height: 1.8;
}

.highlight {
    background-color: rgb(255, 246, 18);
}

.hiddenfile {
 width: 0px;
 height: 0px;
 overflow: hidden;
}

.btn.fadingbutton {
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
  border-bottom: 0;
  position: fixed;
  display: none;
  z-index: 1;
  bottom: 0;
  /* The "Paper" bootstrap theme modifies the transition properties;
  reset them to the default value to prevent ruining the fadeIn() */
  -webkit-transition: all 0s ease 0s;
  -o-transition: all 0s ease 0s;
  transition: all 0s ease 0s;
}
.fadingbutton.back-to-top {
  border-top-right-radius: 0;
  border-right: 0;
  right: 0;
}
.fadingbutton.togglehide {
  border-top-left-radius: 0;
  border-left: 0;
  left: 0;
}

.btn-collapse {
  padding: 4px 10px 1px;
  margin-right: 10px;
  vertical-align: top;
}

.btn:focus, .btn.active:focus {
    outline: none;
    outline: 0;
}

/* Icon when the collapsible content is shown */
.btn-collapse:after {
  font-family: 'Glyphicons Halflings';
  content:"\e082";
}
/* Icon when the collapsible content is hidden */
.btn-collapse.collapsed:after {
  content:"\e081";
}

h1 {
  margin-top: 0;
  margin-bottom: 20px;
}

body.hide_completed .completed {
  display: none !important;
}

input[type="checkbox"]:checked + .item_content {
  text-decoration: line-through;
}

input[type="checkbox"] ~ .glyphicon-eye-close,
input[type="checkbox"] ~ * > .glyphicon-eye-close,
input[type="checkbox"]:checked ~ .glyphicon-eye-open,
input[type="checkbox"]:checked ~ * > .glyphicon-eye-open {
  display: none;
}
input[type="checkbox"] ~ .glyphicon-eye-open,
input[type="checkbox"] ~ * > .glyphicon-eye-open,
input[type="checkbox"]:checked ~ .glyphicon-eye-close,
input[type="checkbox"]:checked ~ * > .glyphicon-eye-close {
  display: inline-block;
}

textarea#profileText {
  height: 15em;
  resize: vertical;
}

/* Work around what seems to be a bootstrap bug affecting the hover border on the right side of the add profile button */
.input-group-btn:last-child>.btn:focus,
.input-group-btn:last-child>.btn:hover {
  z-index: 3;
}

/* Decorators for NG+/NG++ entries */
.s_ng\+ .item_content:before {
  content: "[NG+: ";
}
.s_ng\+\+ .item_content:before {
  content: "[NG++: ";
}
.s_ng\+ .item_content:after,
.s_ng\+\+ .item_content:after {
  content: "]";
}

/* Styling for checklist filter categories and toggles */
.btn-group.btn-group-vertical > .btn-group:not(:first-child) > .btn-group-vertical {
  left: 0;
  top: 100%;
  display: none;
  position: absolute;
}
.btn-group.btn-group-vertical:hover > .btn-group:not(:first-child) > .btn-group-vertical {
  display: block;
}
.btn-group.btn-group-vertical > .btn-group:first-child > .btn-group-vertical.open > .btn {
  z-index: 1;
}
.btn-group.btn-group-vertical > .btn-group:not(:first-child) > .btn-group-vertical > .btn {
  z-index: 3;
  text-align: left;
}
.btn-group.btn-group-vertical > .btn-group:not(:first-child) > .btn-group-vertical > .btn:hover {
  z-index: 4;
}
.btn-group.btn-group-vertical:not(:last-child) > .btn-group:first-child > .btn-group-vertical > .btn {
  border-top-right-radius: 0;
  border-bottom-right-radius: 0;
}
.btn-group.btn-group-vertical:not(:first-child) > .btn-group:first-child > .btn-group-vertical > .btn,
.btn-group.btn-group-vertical > .btn-group:not(:first-child) > .btn-group-vertical > .btn:first-child {
  border-top-left-radius: 0;
}
.btn-group.btn-group-vertical:not(:first-child) > .btn-group:first-child > .btn-group-vertical > .btn,
.btn-group.btn-group-vertical:first-child:hover > .btn-group:first-child > .btn-group-vertical > .btn {
  border-bottom-left-radius: 0;
}
