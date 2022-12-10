---
layout: default
title: Tag Developers Guide
---

# tabbedpanel

> NOTE: Ajax template (Dojo plugin) is deprecated and won't be supported any longer.

__Description__



{% comment %}start snippet id=javadoc|javadoc=true|url=struts2/plugins/dojo/src/main/java/org/apache/struts2/dojo/components/TabbedPanel.java {% endcomment %}
<p> The tabbedpanel widget is primarily an AJAX component, where each tab can either be local content or remote
 content (refreshed each time the user selects that tab).</p>
 If the useSelectedTabCookie attribute is set to true, the id of the selected tab is saved in a cookie on activation.
 When coming back to this view, the cookie is read and the tab will be activated again, unless an actual value for the
 selectedTab attribute is specified.</p>
 If you want to use the cookie feature, please be sure that you provide a unique id for your tabbedpanel component,
 since this will also be the identifying name component of the stored cookie.</p>
</p>
{% comment %}end snippet id=javadoc|javadoc=true|url=struts2/plugins/dojo/src/main/java/org/apache/struts2/dojo/components/TabbedPanel.java {% endcomment %}

__Parameters__



{% comment %}start snippet id=tagattributes|javadoc=false|url=struts2-tags/ajax/a.html {% endcomment %}
<p>		<table width="100%">

			<tr>

				<td colspan="6"><h4>Dynamic Attributes Allowed:</h4> false</td>

			</tr>

			<tr>

				<td colspan="6">&nbsp;</td>

			</tr>

			<tr>

				<th align="left" valign="top"><h4>Name</h4></th>

				<th align="left" valign="top"><h4>Required</h4></th>

				<th align="left" valign="top"><h4>Default</h4></th>

				<th align="left" valign="top"><h4>Evaluated</h4></th>

				<th align="left" valign="top"><h4>Type</h4></th>

				<th align="left" valign="top"><h4>Description</h4></th>

			</tr>

				<tr>

					<td align="left" valign="top">accesskey</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Set the html accesskey attribute on rendered html element</td>

				</tr>

				<tr>

					<td align="left" valign="top">afterNotifyTopics</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Comma delimmited list of topics that will published after the request(if the request succeeds)</td>

				</tr>

				<tr>

					<td align="left" valign="top">ajaxAfterValidation</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">Boolean</td>

					<td align="left" valign="top">Make an asynchronous request if validation succeeds. Only valid if 'validate' is 'true'</td>

				</tr>

				<tr>

					<td align="left" valign="top">beforeNotifyTopics</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Comma delimmited list of topics that will published before the request</td>

				</tr>

				<tr>

					<td align="left" valign="top">cssClass</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">The css class to use for element</td>

				</tr>

				<tr>

					<td align="left" valign="top">cssErrorClass</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">The css error class to use for element</td>

				</tr>

				<tr>

					<td align="left" valign="top">cssErrorStyle</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">The css error style definitions for element to use</td>

				</tr>

				<tr>

					<td align="left" valign="top">cssStyle</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">The css style to use for element</td>

				</tr>

				<tr>

					<td align="left" valign="top">disabled</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Set the html disabled attribute on rendered html element</td>

				</tr>

				<tr>

					<td align="left" valign="top">errorNotifyTopics</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Comma delimmited list of topics that will published after the request(if the request fails)</td>

				</tr>

				<tr>

					<td align="left" valign="top">errorPosition</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Define error position of form element (top|bottom)</td>

				</tr>

				<tr>

					<td align="left" valign="top">errorText</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">The text to display to the user if the is an error fetching the content</td>

				</tr>

				<tr>

					<td align="left" valign="top">executeScripts</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">Boolean</td>

					<td align="left" valign="top">Javascript code in the fetched content will be executed</td>

				</tr>

				<tr>

					<td align="left" valign="top">formFilter</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Function name used to filter the fields of the form.</td>

				</tr>

				<tr>

					<td align="left" valign="top">formId</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Form id whose fields will be serialized and passed as parameters</td>

				</tr>

				<tr>

					<td align="left" valign="top">handler</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Javascript function name that will make the request</td>

				</tr>

				<tr>

					<td align="left" valign="top">highlightColor</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">none</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Color used to perform a highlight effect on the elements specified in the 'targets' attribute</td>

				</tr>

				<tr>

					<td align="left" valign="top">highlightDuration</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">2000</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">Integer</td>

					<td align="left" valign="top">Duration of highlight effect in milliseconds. Only valid if 'highlightColor' attribute is set</td>

				</tr>

				<tr>

					<td align="left" valign="top">href</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">The URL to call to obtain the content. Note: If used with ajax context, the value must be set as an url tag value.</td>

				</tr>

				<tr>

					<td align="left" valign="top">id</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">The id to use for the element</td>

				</tr>

				<tr>

					<td align="left" valign="top">indicator</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Id of element that will be shown while making request</td>

				</tr>

				<tr>

					<td align="left" valign="top">javascriptTooltip</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">Boolean</td>

					<td align="left" valign="top">Use JavaScript to generate tooltips</td>

				</tr>

				<tr>

					<td align="left" valign="top">key</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Set the key (name, value, label) for this particular component</td>

				</tr>

				<tr>

					<td align="left" valign="top">label</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Label expression used for rendering an element specific label</td>

				</tr>

				<tr>

					<td align="left" valign="top">labelSeparator</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">:</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">String that will be appended to the label</td>

				</tr>

				<tr>

					<td align="left" valign="top">labelposition</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Define label position of form element (top/left)</td>

				</tr>

				<tr>

					<td align="left" valign="top">listenTopics</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Topic that will trigger the remote call</td>

				</tr>

				<tr>

					<td align="left" valign="top">loadingText</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">Loading...</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Text to be shown while content is being fetched</td>

				</tr>

				<tr>

					<td align="left" valign="top">name</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">The name to set for element</td>

				</tr>

				<tr>

					<td align="left" valign="top">notifyTopics</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Comma delimmited list of topics that will published before and after the request, and on errors</td>

				</tr>

				<tr>

					<td align="left" valign="top">onblur</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top"> Set the html onblur attribute on rendered html element</td>

				</tr>

				<tr>

					<td align="left" valign="top">onchange</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Set the html onchange attribute on rendered html element</td>

				</tr>

				<tr>

					<td align="left" valign="top">onclick</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Set the html onclick attribute on rendered html element</td>

				</tr>

				<tr>

					<td align="left" valign="top">ondblclick</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Set the html ondblclick attribute on rendered html element</td>

				</tr>

				<tr>

					<td align="left" valign="top">onfocus</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Set the html onfocus attribute on rendered html element</td>

				</tr>

				<tr>

					<td align="left" valign="top">onkeydown</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Set the html onkeydown attribute on rendered html element</td>

				</tr>

				<tr>

					<td align="left" valign="top">onkeypress</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Set the html onkeypress attribute on rendered html element</td>

				</tr>

				<tr>

					<td align="left" valign="top">onkeyup</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Set the html onkeyup attribute on rendered html element</td>

				</tr>

				<tr>

					<td align="left" valign="top">onmousedown</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Set the html onmousedown attribute on rendered html element</td>

				</tr>

				<tr>

					<td align="left" valign="top">onmousemove</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Set the html onmousemove attribute on rendered html element</td>

				</tr>

				<tr>

					<td align="left" valign="top">onmouseout</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Set the html onmouseout attribute on rendered html element</td>

				</tr>

				<tr>

					<td align="left" valign="top">onmouseover</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Set the html onmouseover attribute on rendered html element</td>

				</tr>

				<tr>

					<td align="left" valign="top">onmouseup</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Set the html onmouseup attribute on rendered html element</td>

				</tr>

				<tr>

					<td align="left" valign="top">onselect</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Set the html onselect attribute on rendered html element</td>

				</tr>

				<tr>

					<td align="left" valign="top">openTemplate</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Set template to use for opening the rendered html.</td>

				</tr>

				<tr>

					<td align="left" valign="top">parseContent</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">true</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">Boolean</td>

					<td align="left" valign="top">Parse returned HTML for Dojo widgets</td>

				</tr>

				<tr>

					<td align="left" valign="top">requiredLabel</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">Boolean</td>

					<td align="left" valign="top">If set to true, the rendered element will indicate that input is required</td>

				</tr>

				<tr>

					<td align="left" valign="top">requiredPosition</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Define required position of required form element (left|right)</td>

				</tr>

				<tr>

					<td align="left" valign="top">separateScripts</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">true</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Run scripts in a separate scope, unique for each tag</td>

				</tr>

				<tr>

					<td align="left" valign="top">showErrorTransportText</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">true</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">Boolean</td>

					<td align="left" valign="top">Set whether errors will be shown or not</td>

				</tr>

				<tr>

					<td align="left" valign="top">showLoadingText</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">Boolean</td>

					<td align="left" valign="top">Show loading text on targets</td>

				</tr>

				<tr>

					<td align="left" valign="top">style</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">The css style definitions for element to use - it's an alias of cssStyle attribute.</td>

				</tr>

				<tr>

					<td align="left" valign="top">tabindex</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Set the html tabindex attribute on rendered html element</td>

				</tr>

				<tr>

					<td align="left" valign="top">targets</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Comma delimited list of ids of the elements whose content will be updated</td>

				</tr>

				<tr>

					<td align="left" valign="top">template</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">The template (other than default) to use for rendering the element</td>

				</tr>

				<tr>

					<td align="left" valign="top">templateDir</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">The template directory.</td>

				</tr>

				<tr>

					<td align="left" valign="top">title</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Set the html title attribute on rendered html element</td>

				</tr>

				<tr>

					<td align="left" valign="top">tooltip</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Set the tooltip of this particular component</td>

				</tr>

				<tr>

					<td align="left" valign="top">tooltipConfig</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Deprecated. Use individual tooltip configuration attributes instead.</td>

				</tr>

				<tr>

					<td align="left" valign="top">tooltipCssClass</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">StrutsTTClassic</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">CSS class applied to JavaScrip tooltips</td>

				</tr>

				<tr>

					<td align="left" valign="top">tooltipDelay</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">Classic</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Delay in milliseconds, before showing JavaScript tooltips </td>

				</tr>

				<tr>

					<td align="left" valign="top">tooltipIconPath</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Icon path used for image that will have the tooltip</td>

				</tr>

				<tr>

					<td align="left" valign="top">transport</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">XMLHTTPTransport</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Transport used by Dojo to make the request</td>

				</tr>

				<tr>

					<td align="left" valign="top">validate</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">Boolean</td>

					<td align="left" valign="top">Perform Ajax validation. 'ajaxValidation' interceptor must be applied to action</td>

				</tr>

				<tr>

					<td align="left" valign="top">value</td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top"></td>

					<td align="left" valign="top">false</td>

					<td align="left" valign="top">String</td>

					<td align="left" valign="top">Preset the value of input element.</td>

				</tr>

		</table>

</p>
{% comment %}end snippet id=tagattributes|javadoc=false|url=struts2-tags/ajax/a.html {% endcomment %}

__Examples__

The following is an example of a tabbedpanel and panel tag utilizing local and remote content:


{% comment %}start snippet id=example1|lang=xml|javadoc=true|url=struts2/plugins/dojo/src/main/java/org/apache/struts2/dojo/components/TabbedPanel.java {% endcomment %}

```xml
 <sx:head />
 <sx:tabbedpanel id="test" >
    <sx:div id="one" label="one" theme="ajax" labelposition="top" >
        This is the first pane<br/>
        <s:form>
            <s:textfield name="tt" label="Test Text"/>  <br/>
            <s:textfield name="tt2" label="Test Text2"/>
        </s:form>
    </sx:div>
    <sx:div id="three" label="remote" theme="ajax" href="/AjaxTest.action" >
        This is the remote tab
    </sx:div>
 </sx:tabbedpanel>

```

{% comment %}end snippet id=example1|lang=xml|javadoc=true|url=struts2/plugins/dojo/src/main/java/org/apache/struts2/dojo/components/TabbedPanel.java {% endcomment %}

Use notify topics to prevent a tab from being selected:


{% comment %}start snippet id=example2|lang=xml|javadoc=true|url=struts2/plugins/dojo/src/main/java/org/apache/struts2/dojo/components/TabbedPanel.java {% endcomment %}

```xml
 <sx:head />
 <script type="text/javascript">
 dojo.event.topic.subscribe("/beforeSelect", function(event, tab, tabContainer){
     event.cancel = true;
 });
 </script>
 
 <sx:tabbedpanel id="test" beforeSelectTabNotifyTopics="/beforeSelect">
    <sx:div id="three" label="remote" theme="ajax" href="/AjaxTest.action" >
        One Tab
    </sx:div>
    <sx:div id="three" label="remote" theme="ajax" href="/AjaxTest.action" >
        Another tab
    </sx:div>
 </sx:tabbedpanel>

```

{% comment %}end snippet id=example2|lang=xml|javadoc=true|url=struts2/plugins/dojo/src/main/java/org/apache/struts2/dojo/components/TabbedPanel.java {% endcomment %}