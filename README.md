rofi/config.rasi
nfiguration {
	modi:				"drun";
	font:				"Rubik 10";
	show-icons:                     true;
	icon-theme: 			"Reversal-dark";
	display-drun: 			"";
	drun-display-format:            "{name}";
	sidebar-mode: 			false;
}

* {
	bg: #000000;
	fg: #e8e8d3;
	accent: #687363;
	button: #1c1c1c;
	background-color: @bg;
	text-color: @fg;
	border-color: transparent;
}
window {
	border-radius:                  7px;
	width:			    	50%;
	padding: 			32px;
	background-color:		@bg;
	border:				0px;
}
prompt {
	background-color:		@button;
	enabled:			true;
	padding:			0.5% 32px 0% -0.5%;
	font:				"Rubik 10";
	text-color:			@fg;
}
entry {
    	placeholder:			"Search";
	background-color:               @button;
    	placeholder-color:              @fg;
	text-color:			@fg;
    	expand:                         true;
    	padding:                        0.15% 0% 0% 0%;
}
inputbar {
	children:			[ prompt, entry ];
    	background-color:               @button;
    	expand:                         false;
    	border-radius:                  6px;
    	margin:                         0%;
    	padding:                        10px;
	border:				0px;
}
listview {
    	columns:                        4;
    	lines:	                        3;
    	cycle:                          false;
    	dynamic:                        true;
    	layout:                         vertical;
	border:				0px;
	background-color:		transparent;
}
mainbox {
    	children:                       [ inputbar, listview ];
    	spacing:                       	2%;
    	padding:                        2% 1% 2% 1%;
	border:				0px;
}
element {
    	orientation:                    vertical;
    	padding:                        2% 0% 2% 0%;
	border:				0px;
	background-color:		transparent;
}
element normal.normal, element alternate.normal {
	background-color:		transparent;
	text-color:			@fg;
}
element normal.active, element alternate.active {
	background-color:		transparent;
	text-color:			@fg;
}
element normal.urgent, element alternate.urgent {
	background-color:		transparent;
	text-color:			@fg;
}
element-icon {
    	size:                           48px;
    	horizontal-align:	 	0.5;
}
element-text {
    	expand:                         true;
    	horizontal-align:               0.5;
    	vertical-align:                 0.5;
    	margin:                         0.5% 0.5% -0.5% 0.5%;
}
element-text, element-icon {
	background-color:		inherit;
	text-color:			inherit;
}
element selected.normal, element selected.active, element selected.urgent {
    	background-color:               @button;
    	border-radius:                  6px;
	text-color:			@fg;
	border:				0px;
}
scrollbar {
	handle-color:			@accent;
	background-color:		transparent;
	handle-width:			8px;
	border:				0px;
}
