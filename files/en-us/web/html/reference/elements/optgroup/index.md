---
title: "<optgroup>: The Option Group element"
slug: Web/HTML/Reference/Elements/optgroup
page-type: html-element
browser-compat: html.elements.optgroup
sidebar: htmlsidebar
---

The **`<optgroup>`** [HTML](/en-US/docs/Web/HTML) element creates a grouping of options within a {{HTMLElement("select")}} element.

In [customizable `<select>` elements](/en-US/docs/Learn_web_development/Extensions/Forms/Customizable_select), the {{htmlelement("legend")}} element is allowed as a child of `<optgroup>`, to provide a label that is easy to target and style. This replaces any text set in the `<optgroup>` element's `label` attribute, and it has the same semantics.

{{InteractiveExample("HTML Demo: &lt;optgroup&gt;", "tabbed-standard")}}

```html interactive-example
<label for="dino-select">Choose a dinosaur:</label>
<select id="dino-select">
  <optgroup label="Theropods">
    <option>Tyrannosaurus</option>
    <option>Velociraptor</option>
    <option>Deinonychus</option>
  </optgroup>
  <optgroup label="Sauropods">
    <option>Diplodocus</option>
    <option>Saltasaurus</option>
    <option>Apatosaurus</option>
  </optgroup>
</select>
```

```css interactive-example
label {
  display: block;
  margin-bottom: 10px;
}
```

> [!NOTE]
> Optgroup elements may not be nested.

## Attributes

This element includes the [global attributes](/en-US/docs/Web/HTML/Reference/Global_attributes).

- [`disabled`](/en-US/docs/Web/HTML/Reference/Attributes/disabled)
  - : If this Boolean attribute is set, none of the items in this option group is selectable. Often browsers grey out such control and it won't receive any browsing events, like mouse clicks or focus-related ones.
- `label`
  - : The name of the group of options, which the browser can use when labeling the options in the user interface. This attribute is mandatory if this element is used.

## Examples

```html
<select>
  <optgroup label="Group 1">
    <option>Option 1.1</option>
  </optgroup>
  <optgroup label="Group 2">
    <option>Option 2.1</option>
    <option>Option 2.2</option>
  </optgroup>
  <optgroup label="Group 3" disabled>
    <option>Option 3.1</option>
    <option>Option 3.2</option>
    <option>Option 3.3</option>
  </optgroup>
</select>
```

### Result

{{EmbedLiveSample("Examples")}}

## Technical summary

<table class="properties">
  <tbody>
    <tr>
      <th scope="row">
        <a href="/en-US/docs/Web/HTML/Guides/Content_categories"
          >Content categories</a
        >
      </th>
      <td>None.</td>
    </tr>
    <tr>
      <th scope="row">Permitted content</th>
      <td>Zero or more {{HTMLElement("option")}} elements. In <a href="/en-US/docs/Learn_web_development/Extensions/Forms/Customizable_select">customizable select elements</a>, a {{htmlelement("legend")}} element is permitted as a child of <code>&lt;optgroup&gt;</code>.</td>
    </tr>
    <tr>
      <th scope="row">Tag omission</th>
      <td>
        The start tag is mandatory. The end tag is optional if this element is
        immediately followed by another <code>&#x3C;optgroup></code> element, or
        if the parent element has no more content.
      </td>
    </tr>
    <tr>
      <th scope="row">Permitted parents</th>
      <td>A {{HTMLElement("select")}} element.</td>
    </tr>
    <tr>
      <th scope="row">Implicit ARIA role</th>
      <td><a href="/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/group_role"><code>group</code></a></td>
    </tr>
    <tr>
      <th scope="row">Permitted ARIA roles</th>
      <td>No <code>role</code> permitted</td>
    </tr>
    <tr>
      <th scope="row">DOM interface</th>
      <td>{{domxref("HTMLOptGroupElement")}}</td>
    </tr>
  </tbody>
</table>

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- Other form-related elements: {{HTMLElement("form")}}, {{HTMLElement("legend")}}, {{HTMLElement("label")}}, {{HTMLElement("button")}}, {{HTMLElement("select")}}, {{HTMLElement("datalist")}}, {{HTMLElement("option")}}, {{HTMLElement("fieldset")}}, {{HTMLElement("textarea")}}, {{HTMLElement("input")}}, {{HTMLElement("output")}}, {{HTMLElement("progress")}} and {{HTMLElement("meter")}}.
- [Customizable select elements](/en-US/docs/Learn_web_development/Extensions/Forms/Customizable_select)
