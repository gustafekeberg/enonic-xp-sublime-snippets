# enonic-xp-sublime-snippets

Sublime Text 3 snippets for Enonic XP

Included snippets:

## content-type.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<?xml version="1.0" encoding="UTF-8"?>
<content-type>
  <display-name>$1</display-name>
  ${2:<content-display-name-script>\$('$3', '$4')</content-display-name-script>}
  <super-type>${5:base:structured}</super-type>
  <is-abstract>${6:false}</is-abstract>
  <is-final>${7:true}</is-final>
  <allow-child-content>${8:true}</allow-child-content>
  <form>
    $0
  </form>
</content-type>
]]></content>
  <tabTrigger>xpContentType</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - Content Type</description>
</snippet>
```

## field-set.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<field-set name="$1">
  <label>$2</label>
  <items>
    ${3:$SELECTION}
  </items>
</field-set>
]]></content>
  <tabTrigger>xpFieldSet</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - Field Set</description>
</snippet>
```

## filters.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<filters>
  ${1:$SELECTION}
</filters>
]]></content>
  <tabTrigger>xpFilters</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - Filters</description>
</snippet>
```

## inline.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<inline mixin="$1"/>
]]></content>
  <tabTrigger>xpInline</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - inline</description>
</snippet>
```

## input-AttachmentUploader.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<input name="$1" type="AttachmentUploader">
  <label>$2</label>
  <occurrences minimum="$3" maximum="$4"/>
  <config/>
</input>
]]></content>
  <tabTrigger>xpAttachmentUploader</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - AttachmentUploader</description>
</snippet>
```

## input-CheckBox.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<input name="$1" type="CheckBox">
  <label>$2</label>
  <occurrences minimum="0" maximum="1"/>
  <default>${3:checked}</default>
</input>
]]></content>
  <tabTrigger>xpCheckBox</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - CheckBox</description>
</snippet>
```

## input-ComboBox.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<input name="$1" type="ComboBox">
  <label>$2</label>
  <occurrences minimum="$3" maximum="$4"/>
  <config>
    <option value="$5">$6</option>
  </config>
  <default>$5</default>
</input>
]]></content>
  <tabTrigger>xpComboBox</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - ComboBox</description>
</snippet>
```

## input-ContentSelector.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<input name="$1" type="ContentSelector">
  <label>$2</label>
  <occurrences minimum="$3" maximum="$4"/>
  <config>
    <relationship>system:reference</relationship>
    <allowType>$5</allowType>
    <allowPath>\${site\}/$6/</allowPath>
  </config>
</input>
]]></content>
  <tabTrigger>xpContentSelector</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - ContentSelector</description>
</snippet>
```

## input-Date.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<input name="$1" type="Date">
  <label>$2</label>
  <occurrences minimum="$3" maximum="$4"/>
  <config>
    <timezone>${5:true}</timezone>
  </config>
</input>
]]></content>
  <tabTrigger>xpDate</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - Date</description>
</snippet>
```

## input-DateTime.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<input name="$1" type="DateTime">
  <label>$2</label>
  <occurrences minimum="$3" maximum="$4"/>
  <config>
    <timezone>${5:true}</timezone>
  </config>
</input>
]]></content>
  <tabTrigger>xpDateTime</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - DateTime</description>
</snippet>
```

## input-Double.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<input name="$1" type="Double">
  <label>$2</label>
  <default>${3:3.14159265359}</default>
</input>
]]></content>
  <tabTrigger>xpDouble</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - Double</description>
</snippet>
```

## input-GeoPoint.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<input name="$1" type="GeoPoint">
  <label>$2</label>
  <occurrences minimum="$3" maximum="$4"/>
</input>
]]></content>
  <tabTrigger>xpGeoPoint</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - GeoPoint</description>
</snippet>
```

## input-HtmlArea.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<input name="$1" type="HtmlArea">
  <label>$2</label>
  <default>${3:<h3>Enter data for `$1` here</h3>}</default>
</input>
]]></content>
  <tabTrigger>xpHtmlArea</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - HtmlArea</description>
</snippet>
```

## input-ImageSelector.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<input name="$1" type="ImageSelector">
  <label>$2</label>
  <occurrences minimum="$3" maximum="$4"/>
  <config>
    <allowPath>${5:./*}</allowPath>
  </config>
</input>
]]></content>
  <tabTrigger>xpImageSelector</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - ImageSelector</description>
</snippet>
```

## input-Long.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<input name="$1" type="Long">
  <label>$2</label>
  <default>${3:42}</default>
</input>
]]></content>
  <tabTrigger>xpLong</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - Long</description>
</snippet>
```

## input-RadioButton.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<input name="$1" type="RadioButton">
  <label>$2</label>
  <occurrences minimum="$3" maximum="$4"/>
  <config>
    <option value="$5">$6</option>
  </config>
  <default>$5</default>
</input>
]]></content>
  <tabTrigger>xpRadioButton</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - RadioButton</description>
</snippet>
```

## input-Tag.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<input name="$1" type="Tag">
  <label>$2</label>
  <occurrences minimum="$3" maximum="$4"/>
</input>
]]></content>
  <tabTrigger>xpTag</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - Tag</description>
</snippet>
```

## input-TextArea.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<input name="$1" type="TextArea">
  <label>$2</label>
  <default>${3:Description goes here}</default>
</input>
]]></content>
  <tabTrigger>xpTextArea</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - TextArea</description>
</snippet>
```

## input-TextLine.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<input name="$1" type="TextLine">
  <label>$2</label>
  <occurrences minimum="$3" maximum="$4"/>
  <config>
    <regexp>$5</regexp>
  </config>
  <default>$6</default>
</input>
]]></content>
  <tabTrigger>xpTextLine</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - TextLine</description>
</snippet>
```

## input-Time.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<input name="$1" type="Time">
  <label>$2</label>
  <occurrences minimum="$3" maximum="$4"/>
</input>
]]></content>
  <tabTrigger>xpTime</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - Time</description>
</snippet>
```

## item-set.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<item-set name="$1">
  <label>$2</label>
  <occurrences minimum="$3" maximum="$4"/>
  <items>
    ${0:$SELECTION}
  </items>
</item-set>
]]></content>
  <tabTrigger>xpItemSet</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - Item Set</description>
</snippet>
```

## layout.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<?xml version="1.0" encoding="UTF-8"?>
<layout>
  <display-name>$1</display-name>
  <config/>
  <regions>
    <region name="$2"/>
  </regions>
</layout>
]]></content>
  <tabTrigger>xpLayout</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - Layout</description>
</snippet>
```

## mapping.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<mapping controller="$1">
  <match>${2:type:'portal:fragment'}</match>
  ${3:<pattern invert="${4:true}">${5:.*\/_\/.*}</pattern>}
</mapping>
]]></content>
  <tabTrigger>xpMapping</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - Mapping</description>
</snippet>
```

## mappings.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<mappings>
  ${1:$SELECTION}
</mappings>
]]></content>
  <tabTrigger>xpMappings</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - Mappings</description>
</snippet>
```

## mixin.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<?xml version="1.0" encoding="UTF-8"?>
<mixin>
  <display-name>$1</display-name>
  <items>
    $0
  </items>
</mixin>
]]></content>
  <tabTrigger>xpMixin</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - Mixin</description>
</snippet>
```

## page.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<?xml version="1.0" encoding="UTF-8"?>
<page>
  <display-name>$1</display-name>
  <config>
    $3
  </config>
  <regions>
    <region name="$2"/>
  </regions>
</page>
]]></content>
  <tabTrigger>xpPage</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - Page</description>
</snippet>
```

## part.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<?xml version="1.0" encoding="UTF-8"?>
<part>
  <display-name>$1</display-name>
  <config>
    <field-set name="$2">
      <label>$3</label>
      <items>
        $0
      </items>
    </field-set>
  </config>
</part>
]]></content>
  <tabTrigger>xpPart</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - Part</description>
</snippet>
```

## response-filter.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<response-filter name="$1" order="$2"/>
]]></content>
  <tabTrigger>xpResponseFilter</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - Response Filter</description>
</snippet>
```

## site.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<?xml version="1.0" encoding="UTF-8"?>
<site>
  ${1:<filters>
    $2
  </filters>}
  ${3:<mappings>
    $4
  </mappings>}
  ${5:<x-data mixin="$6"/>}
  ${7:<config>
    $8
  </config>}
</site>
]]></content>
  <tabTrigger>xpSite</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - Site</description>
</snippet>
```

## x-data.sublime-snippet

```xml
<snippet>
  <content><![CDATA[
<x-data mixin="$1"/>
]]></content>
  <tabTrigger>xpXData</tabTrigger>
  <scope>text.xml</scope>
  <description>Enonic XP - x-data</description>
</snippet>
```
