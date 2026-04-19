# <a name="document-top"></a>Buffer Accessibility Conformance Report

<b>VPAT® Version 2.5 — International Edition</b>

<b>Name of Product:</b> Buffer

<b>Platform:</b> Web

<b>Date:</b> April 2026

<b>Contact Information:</b> <a href="mailto:accessibility@buffer.com">accessibility@buffer.com</a>

<b>Notes:</b> This report covers accessibility conformance for the Buffer web application, which includes the product suite Publish, Analyze, and Start Page.

<b>Evaluation Methods Used:</b> Conformance to the listed accessibility standards has been evaluated through a combination of self-assessment (design-side audit using Stark, engineering code review, and manual testing with macOS VoiceOver + Safari). Automated scans were performed using Axe.

<b>Applicable Standards/Guidelines:</b>

<table>
  <thead>
    <tr>
      <th>Standard/Guideline</th>
      <th>Included in Report</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21">Web Content Accessibility Guidelines 2.1</a></td>
      <td>Level AA (Yes)</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG22/">Web Content Accessibility Guidelines 2.2</a></td>
      <td>Level AA (Yes)</td>
    </tr>
    <tr>
      <td><a href="https://www.access-board.gov/ict/">Revised Section 508 standards</a></td>
      <td>Yes</td>
    </tr>
    <tr>
      <td><a href="https://www.etsi.org/deliver/etsi_en/301500_301599/301549/03.02.01_60/en_301549v030201p.pdf">EN 301 549 Accessibility requirements for ICT products and services — V3.2.1 (2021-03)</a></td>
      <td>Yes</td>
    </tr>
  </tbody>
</table>

## Terms

The terms used in the Conformance Level information are defined as follows:

<ul>
  <li><b>Supports:</b> The functionality of the product has at least one method that meets the criterion without known defects or meets with equivalent facilitation.</li>
  <li><b>Partially Supports:</b> Some functionality of the product does not meet the criterion.</li>
  <li><b>Does Not Support:</b> The majority of product functionality does not meet the criterion.</li>
  <li><b>Not Applicable:</b> The criterion is not relevant to the product.</li>
  <li><b>Not Evaluated:</b> The product has not been evaluated against the criterion. This can only be used in WCAG Level AAA criteria.</li>
</ul>

---

## WCAG 2.x Report

The WCAG criteria below are applicable to the following standards:

- EN 301 549: Clause 9 (Web), Clause 10 (Non-web Documents), Clause 11 (Software)
- Revised Section 508: Chapter 5 — 501.1 Scope and 504.2 Content Creation or Editing; Chapter 6 — 602.3 Electronic Support Documentation

### Table 1: Success Criteria, Level A

<table>
  <thead>
    <tr>
      <th width="30%" scope="col">Criteria</th>
      <th width="20%" scope="col">Conformance Level</th>
      <th width="50%" scope="col">Remarks and Explanations</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#non-text-content">1.1.1 Non-text Content</a> (Level A)</td>
      <td>Partially Supports</td>
      <td>Most decorative and non-decorative images are handled appropriately. Some SVG images in Analyze have an image role but do not provide accessible text alternatives.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#audio-only-and-video-only-prerecorded">1.2.1 Audio-only and Video-only (Prerecorded)</a> (Level A)</td>
      <td>Not Applicable</td>
      <td>No audio-only or video-only prerecorded content is used. Short feature announcement videos are synchronized media and are addressed under captions and audio description criteria.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#captions-prerecorded">1.2.2 Captions (Prerecorded)</a> (Level A)</td>
      <td>Supports</td>
      <td>Feature announcement videos include captions, though users may need to enable them manually.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#audio-description-or-media-alternative-prerecorded">1.2.3 Audio Description or Media Alternative (Prerecorded)</a> (Level A)</td>
      <td>Supports</td>
      <td>Feature announcement videos do not rely on visual-only information that requires audio description or a separate media alternative.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#info-and-relationships">1.3.1 Info and Relationships</a> (Level A)</td>
      <td>Partially Supports</td>
      <td>Most pages are missing a semantic H1 heading, and some list structures in Publish — including the Community, Insights, and Create sections — and Start Page are not programmatically structured correctly. Other structural relationships, including form labels and tables, are generally programmatically conveyed.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#meaningful-sequence">1.3.2 Meaningful Sequence</a> (Level A)</td>
      <td>Supports</td>
      <td>Reading order matches the visual presentation across all product areas.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#sensory-characteristics">1.3.3 Sensory Characteristics</a> (Level A)</td>
      <td>Supports</td>
      <td>Instructions and content do not rely solely on shape, size, visual location, or orientation.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#use-of-color">1.4.1 Use of Color</a> (Level A)</td>
      <td>Partially Supports</td>
      <td>Error states, status badges, and most interactive states include non-color identifiers such as icons and text labels. Some links in Settings areas, including Tags and Apps &amp; Extras, are only distinguishable from surrounding text by color.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#audio-control">1.4.2 Audio Control</a> (Level A)</td>
      <td>Not Applicable</td>
      <td>Product does not include audio that plays automatically.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#keyboard">2.1.1 Keyboard</a> (Level A)</td>
      <td>Partially Supports</td>
      <td>Most functionality is operable through a keyboard interface, and drag-to-reorder interactions include keyboard or menu alternatives. Some legacy controls in Analyze and Start Page may not be fully keyboard accessible.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#no-keyboard-trap">2.1.2 No Keyboard Trap</a> (Level A)</td>
      <td>Supports</td>
      <td>Focus can be moved away from interactive components using standard keyboard navigation. Modals trap focus while open and release focus when closed.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#character-key-shortcuts">2.1.4 Character Key Shortcuts</a> (Level A — WCAG 2.1)</td>
      <td>Does Not Support</td>
      <td>The publishing area includes single-character shortcut sequences that cannot be turned off or remapped. These shortcuts are suppressed in input fields, but no global disable or remap mechanism is provided.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#timing-adjustable">2.2.1 Timing Adjustable</a> (Level A)</td>
      <td>Partially Supports</td>
      <td>Session timeouts exceed 20 hours and qualify for the WCAG exemption. Some auto-dismissing notifications, including actionable toasts, may disappear before keyboard or screen reader users can act.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#pause-stop-hide">2.2.2 Pause, Stop, Hide</a> (Level A)</td>
      <td>Partially Supports</td>
      <td>Toast notifications auto-dismiss and may be missed by users who cannot reach them in time. Error toasts are announced to assistive technologies, but non-error notifications are not consistently announced.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#three-flashes-or-below-threshold">2.3.1 Three Flashes or Below Threshold</a> (Level A)</td>
      <td>Not Applicable</td>
      <td>Product does not contain content that flashes more than three times per second.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#bypass-blocks">2.4.1 Bypass Blocks</a> (Level A)</td>
      <td>Supports</td>
      <td>A skip-to-main-content link is available as the first focusable element in Publish, Analyze, and Start Page.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#page-titled">2.4.2 Page Titled</a> (Level A)</td>
      <td>Partially Supports</td>
      <td>Most main flows use descriptive page titles. Some start page and login views fall back to generic titles that do not identify the current page or section.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#focus-order">2.4.3 Focus Order</a> (Level A)</td>
      <td>Supports</td>
      <td>Focus order follows the visual layout and logical reading sequence. The channel list has two focus points per row by design; order is intentional and consistent.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#link-purpose-in-context">2.4.4 Link Purpose (In Context)</a> (Level A)</td>
      <td>Partially Supports</td>
      <td>Most links are descriptive or shown with meaningful surrounding context. Some links in Start Page and Analyze do not have discernible accessible text.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#pointer-gestures">2.5.1 Pointer Gestures</a> (Level A — WCAG 2.1)</td>
      <td>Supports</td>
      <td>Drag-to-reorder channels includes an alternative via menu. No swipe-only or pinch-only interactions are in use.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#pointer-cancellation">2.5.2 Pointer Cancellation</a> (Level A — WCAG 2.1)</td>
      <td>Supports</td>
      <td>All interactive elements use standard click events. No critical actions trigger on mousedown or touchstart.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#label-in-name">2.5.3 Label in Name</a> (Level A — WCAG 2.1)</td>
      <td>Partially Supports</td>
      <td>Most icon-only controls have accessible names that match their visible labels or purpose. Some controls in Analyze and Start Page are missing accessible names or have label mismatches.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#motion-actuation">2.5.4 Motion Actuation</a> (Level A — WCAG 2.1)</td>
      <td>Not Applicable</td>
      <td>Product does not use device motion or user motion for any functionality.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#language-of-page">3.1.1 Language of Page</a> (Level A)</td>
      <td>Supports</td>
      <td>All pages across the product include a properly declared lang="en" attribute on the &lt;html&gt; element.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#on-focus">3.2.1 On Focus</a> (Level A)</td>
      <td>Supports</td>
      <td>No navigation, form submission, or dialogs are triggered on focus alone.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#on-input">3.2.2 On Input</a> (Level A)</td>
      <td>Supports</td>
      <td>No unexpected context changes occur when interacting with any input controls.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG22/#consistent-help">3.2.6 Consistent Help</a> (Level A — WCAG 2.2)</td>
      <td>Supports</td>
      <td>Help options appear consistently across authenticated product areas. Pre-authentication pages use inline support links in varying positions.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#error-identification">3.3.1 Error Identification</a> (Level A)</td>
      <td>Partially Supports</td>
      <td>Most errors identify the affected field or action. Generic fallback errors may not clearly identify what failed or what the user can do next.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#labels-or-instructions">3.3.2 Labels or Instructions</a> (Level A)</td>
      <td>Partially Supports</td>
      <td>Most form inputs include visible labels and instructions. Some password requirements are presented after the input, which can make them harder for screen reader users to discover before entry.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG22/#redundant-entry">3.3.7 Redundant Entry</a> (Level A — WCAG 2.2)</td>
      <td>Supports</td>
      <td>Multi-step processes collect distinct data per step and preserve previously entered information. Password re-entry for sensitive actions is exempt as essential for security. No redundant entry patterns were found.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#parsing">4.1.1 Parsing</a> (Level A)</td>
      <td>Not Applicable</td>
      <td>Obsoleted in WCAG 2.2; automatically satisfied per W3C guidance.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#name-role-value">4.1.2 Name, Role, Value</a> (Level A)</td>
      <td>Partially Supports</td>
      <td>Most newer interface elements expose appropriate names, roles, states, and keyboard behavior. Some interface elements use unsupported or invalid ARIA attributes, nested interactive controls, missing button names, invalid ARIA parent/child relationships, or do not fully expose state.</td>
    </tr>
  </tbody>
</table>

### Table 2: Success Criteria, Level AA

<table>
  <thead>
    <tr>
      <th width="30%" scope="col">Criteria</th>
      <th width="20%" scope="col">Conformance Level</th>
      <th width="50%" scope="col">Remarks and Explanations</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#captions-live">1.2.4 Captions (Live)</a> (Level AA)</td>
      <td>Not Applicable</td>
      <td>Product does not include live audio content.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#audio-description-prerecorded">1.2.5 Audio Description (Prerecorded)</a> (Level AA)</td>
      <td>Supports</td>
      <td>Feature announcement videos do not rely on visual-only information that requires audio description.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#orientation">1.3.4 Orientation</a> (Level AA — WCAG 2.1)</td>
      <td>Supports</td>
      <td>Content is not restricted to a single display orientation.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#identify-input-purpose">1.3.5 Identify Input Purpose</a> (Level AA — WCAG 2.1)</td>
      <td>Does Not Support</td>
      <td>Most fields that collect user information do not include appropriate autocomplete attributes, including email and password fields in login, signup, and password reset flows. Payment fields are provided by Stripe and are out of scope.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#contrast-minimum">1.4.3 Contrast (Minimum)</a> (Level AA)</td>
      <td>Partially Supports</td>
      <td>Most text meets minimum contrast requirements. Some text in Settings, Insights, and Billing, including some badge labels and UI text, does not meet minimum contrast requirements.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#resize-text">1.4.4 Resize Text</a> (Level AA)</td>
      <td>Partially Supports</td>
      <td>Most content is usable at 200% zoom. Some account menu and Publish header controls overflow or are cut off at high zoom or small viewport sizes.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#images-of-text">1.4.5 Images of Text</a> (Level AA)</td>
      <td>Supports</td>
      <td>Buffer does not use images of text except for logos and brand elements, which are exempt.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#reflow">1.4.10 Reflow</a> (Level AA — WCAG 2.1)</td>
      <td>Partially Supports</td>
      <td>Most surrounding UI reflows at narrow widths. Some Publish header controls are cut off, and Analyze and Start Page layouts do not fully adapt; calendar and board views require two-dimensional layout.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#non-text-contrast">1.4.11 Non-text Contrast</a> (Level AA — WCAG 2.1)</td>
      <td>Supports</td>
      <td>Icons and form field boundaries generally meet the required 3:1 contrast ratio. Decorative borders on some tertiary icon buttons are below 3:1 but do not convey state or meaning.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#text-spacing">1.4.12 Text Spacing</a> (Level AA — WCAG 2.1)</td>
      <td>Partially Supports</td>
      <td>Most product areas allow user text spacing overrides. Some sidebar and small-label styles prevent or limit line-height overrides required by this criterion.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#content-on-hover-or-focus">1.4.13 Content on Hover or Focus</a> (Level AA — WCAG 2.1)</td>
      <td>Supports</td>
      <td>Tooltips remain visible while hovering and are dismissible without moving focus.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#multiple-ways">2.4.5 Multiple Ways</a> (Level AA)</td>
      <td>Partially Supports</td>
      <td>Sidebar navigation and the command palette provide multiple ways to navigate. The command palette is not always available through a visible mouse or touch trigger.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#headings-and-labels">2.4.6 Headings and Labels</a> (Level AA)</td>
      <td>Partially Supports</td>
      <td>Some page headings identify only the selected channel and not the active feature area. This can make headings less descriptive for screen reader users.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#focus-visible">2.4.7 Focus Visible</a> (Level AA)</td>
      <td>Supports</td>
      <td>A clear high-contrast focus ring is displayed on all keyboard-focusable interactive elements throughout the product.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG22/#focus-not-obscured-minimum">2.4.11 Focus Not Obscured (Minimum)</a> (Level AA — WCAG 2.2)</td>
      <td>Supports</td>
      <td>Focused elements are not entirely hidden by other content.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG22/#dragging-movements">2.5.7 Dragging Movements</a> (Level AA — WCAG 2.2)</td>
      <td>Supports</td>
      <td>Drag-to-reorder interactions for channels and media include alternatives via buttons and keyboard.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG22/#target-size-minimum">2.5.8 Target Size (Minimum)</a> (Level AA — WCAG 2.2)</td>
      <td>Supports</td>
      <td>Interactive targets meet the 24px minimum, and touch targets increase on touch devices.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#language-of-parts">3.1.2 Language of Parts</a> (Level AA)</td>
      <td>Does Not Support</td>
      <td>User-generated posts and comments may be in languages other than English, but content-level language is not identified. Some localized product content also does not update the page language declaration.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#consistent-navigation">3.2.3 Consistent Navigation</a> (Level AA)</td>
      <td>Supports</td>
      <td>Navigation order is consistent across all pages, established through the recent product redesign.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#consistent-identification">3.2.4 Consistent Identification</a> (Level AA)</td>
      <td>Partially Supports</td>
      <td>The same channel-connection function is labeled inconsistently in different product areas.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#error-suggestion">3.3.3 Error Suggestion</a> (Level AA)</td>
      <td>Partially Supports</td>
      <td>Most error messages identify failures and suggest corrections where possible. Some fallback and login errors do not provide clear corrective guidance.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#error-prevention-legal-financial-data">3.3.4 Error Prevention (Legal, Financial, Data)</a> (Level AA)</td>
      <td>Supports</td>
      <td>Confirmation dialogs are presented before critical or destructive actions, including deleting channels and canceling subscriptions.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG22/#accessible-authentication-minimum">3.3.8 Accessible Authentication (Minimum)</a> (Level AA — WCAG 2.2)</td>
      <td>Partially Supports</td>
      <td>Password fields accept paste and can be used with browser password managers, but most are missing explicit autocomplete attributes. Signup uses invisible hCaptcha, which may fall back to a visual challenge without an accessible alternative.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#status-messages">4.1.3 Status Messages</a> (Level AA — WCAG 2.1)</td>
      <td>Partially Supports</td>
      <td>Most product notifications and form errors are announced or associated with their related fields. Some login errors are visually displayed without live-region or field association support.</td>
    </tr>
  </tbody>
</table>

### Table 3: Success Criteria, Level AAA

This report does not include Level AAA criteria. Buffer is reporting against WCAG 2.2 Level AA, including WCAG 2.1 Level AA criteria.

---

## Revised Section 508 Report

### Chapter 3: Functional Performance Criteria

<table>
  <thead>
    <tr>
      <th width="30%" scope="col">Criteria</th>
      <th width="20%" scope="col">Conformance Level</th>
      <th width="50%" scope="col">Remarks and Explanations</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>302.1 Without Vision</td>
      <td>Partially Supports</td>
      <td>Core product functionality has been reviewed with macOS VoiceOver and screen reader users can navigate and operate primary features. However, known gaps in accessible names, semantic structure, and interaction state exposure (see 4.1.2, 2.5.3, and 1.3.1) mean some controls and page regions are not fully accessible without vision.</td>
    </tr>
    <tr>
      <td>302.2 With Limited Vision</td>
      <td>Partially Supports</td>
      <td>Most text contrast, zoom, and spacing behavior is supported. Some badge labels have insufficient contrast, some controls overflow at high zoom, and some layouts or text styles do not fully adapt to user settings.</td>
    </tr>
    <tr>
      <td>302.3 Without Perception of Color</td>
      <td>Partially Supports</td>
      <td>Most status indicators and interactive states include non-color identifiers. Some insight and analytics charts rely on color alone to distinguish data series.</td>
    </tr>
    <tr>
      <td>302.4 Without Hearing</td>
      <td>Supports</td>
      <td>Audio information in feature announcement videos is provided through captions or on-screen text. The product does not rely on audio for core operation.</td>
    </tr>
    <tr>
      <td>302.5 With Limited Hearing</td>
      <td>Supports</td>
      <td>Audio information in feature announcement videos is provided through captions or on-screen text. The product does not rely on audio for core operation.</td>
    </tr>
    <tr>
      <td>302.6 Without Speech</td>
      <td>Not Applicable</td>
      <td>Product does not require speech input for any functionality.</td>
    </tr>
    <tr>
      <td>302.7 With Limited Manipulation</td>
      <td>Partially Supports</td>
      <td>The command palette is not always available through a visible mouse or touch trigger, which can limit access for users who do not use keyboard shortcuts.</td>
    </tr>
    <tr>
      <td>302.8 With Limited Reach and Strength</td>
      <td>Not Applicable</td>
      <td>Buffer is a web application and does not include physical hardware requiring reach or strength.</td>
    </tr>
    <tr>
      <td>302.9 With Limited Language, Cognitive, and Learning Abilities</td>
      <td>Partially Supports</td>
      <td>Navigation and error messaging are generally consistent and understandable. Some repeated functions use inconsistent labels, some page titles are generic, and some error messages lack suggested corrections.</td>
    </tr>
  </tbody>
</table>

### Chapter 4: Hardware

Buffer is a web application accessed through standard web browsers. It does not include hardware components. All Chapter 4 criteria are Not Applicable.

### Chapter 5: Software

<table>
  <thead>
    <tr>
      <th width="30%" scope="col">Criteria</th>
      <th width="20%" scope="col">Conformance Level</th>
      <th width="50%" scope="col">Remarks and Explanations</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>501.1 Scope — Incorporation of WCAG 2.0 AA</td>
      <td>See <a href="#document-top">WCAG 2.x</a> section</td>
      <td>See information in WCAG 2.x section above.</td>
    </tr>
    <tr>
      <td>502 Interoperability with Assistive Technology</td>
      <td>See <a href="#document-top">WCAG 2.x</a> section</td>
      <td>Buffer is a web application. Assistive technology interoperability is addressed through WCAG criteria (particularly 4.1.2 Name, Role, Value). Section 502 criteria relating to platform accessibility services apply to native software and are addressed through the browser platform.</td>
    </tr>
    <tr>
      <td>503.2 User Preferences</td>
      <td>Supports</td>
      <td>Buffer respects user-configured browser and OS accessibility preferences including font size, high contrast mode, and reduced motion.</td>
    </tr>
    <tr>
      <td>503.3 Alternative User Interfaces</td>
      <td>Not Applicable</td>
      <td>Product does not provide alternative user interfaces.</td>
    </tr>
    <tr>
      <td>503.4 User Controls for Captions and Audio Description</td>
      <td>Supports</td>
      <td>Feature announcement videos include user controls for captions where captions are available. The product does not include media requiring separate audio description controls.</td>
    </tr>
    <tr>
      <td>504.2 Content Creation or Editing</td>
      <td>Supports</td>
      <td>Buffer is an authoring tool for social media content. Alt text input is available wherever the destination platform supports it. Support varies by social media channel.</td>
    </tr>
    <tr>
      <td>504.2.1 Preservation of Information in Format Conversion</td>
      <td>Partially Supports</td>
      <td>Alt text entered for supported image posts is preserved through publishing to destination platforms. Alt text is not supported for all media formats, and exported analytics PDFs do not preserve semantic structure or chart alternatives.</td>
    </tr>
    <tr>
      <td>504.2.2 PDF Export</td>
      <td>Does Not Support</td>
      <td>Exported analytics PDFs are not optimized for accessibility. They lack tagged PDF structure, defined reading order, and text alternatives for charts.</td>
    </tr>
    <tr>
      <td>504.3 Prompts</td>
      <td>Does Not Support</td>
      <td>Buffer provides alt text input fields for supported image posts. The product does not warn, prompt, or require authors to add alt text before publishing.</td>
    </tr>
    <tr>
      <td>504.4 Templates</td>
      <td>Not Applicable</td>
      <td>Product does not provide document templates.</td>
    </tr>
  </tbody>
</table>

### Chapter 6: Support Documentation and Services

<table>
  <thead>
    <tr>
      <th width="30%" scope="col">Criteria</th>
      <th width="20%" scope="col">Conformance Level</th>
      <th width="50%" scope="col">Remarks and Explanations</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>602.2 Accessibility and Compatibility Features</td>
      <td>Partially Supports</td>
      <td>Accessibility features, including alt text support, are documented in the Help Center and at <a href="https://buffer.com/accessibility">buffer.com/accessibility</a>. Documentation is not yet comprehensive across all product areas.</td>
    </tr>
    <tr>
      <td>602.3 Electronic Support Documentation</td>
      <td>See <a href="#document-top">WCAG 2.x</a> section</td>
      <td>See information in WCAG 2.x section above.</td>
    </tr>
    <tr>
      <td>602.4 Alternate Formats for Non-Electronic Support Documentation</td>
      <td>Not Applicable</td>
      <td>All support documentation is provided electronically.</td>
    </tr>
    <tr>
      <td>603.2 Information on Accessibility and Compatibility Features</td>
      <td>Partially Supports</td>
      <td>Support staff can provide information on accessibility features, and the Accessibility Statement provides a public overview. More detailed feature documentation is still needed.</td>
    </tr>
    <tr>
      <td>603.3 Accommodation of Communication Needs</td>
      <td>Partially Supports</td>
      <td>Customer support is provided through text-based channels. Known accessibility issues in the chat widget may prevent some screen reader users from accessing answers.</td>
    </tr>
  </tbody>
</table>

---

## EN 301 549 Report

### Clause 4: Functional Performance Statements

<table>
  <thead>
    <tr>
      <th width="30%" scope="col">Criteria</th>
      <th width="20%" scope="col">Conformance Level</th>
      <th width="50%" scope="col">Remarks and Explanations</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>4.2.1 Usage without vision</td>
      <td>Partially Supports</td>
      <td>See Section 508 criterion 302.1.</td>
    </tr>
    <tr>
      <td>4.2.2 Usage with limited vision</td>
      <td>Partially Supports</td>
      <td>Most text contrast, zoom, and spacing behavior is supported. Some badge labels have insufficient contrast, some controls overflow at high zoom, and some layouts or text styles do not fully adapt to user settings.</td>
    </tr>
    <tr>
      <td>4.2.3 Usage without perception of colour</td>
      <td>Partially Supports</td>
      <td>See Section 508 criterion 302.3.</td>
    </tr>
    <tr>
      <td>4.2.4 Usage without hearing</td>
      <td>Supports</td>
      <td>See Section 508 criterion 302.4.</td>
    </tr>
    <tr>
      <td>4.2.5 Usage with limited hearing</td>
      <td>Supports</td>
      <td>See Section 508 criterion 302.5.</td>
    </tr>
    <tr>
      <td>4.2.6 Usage with no or limited vocal capability</td>
      <td>Not Applicable</td>
      <td>Product does not require speech input.</td>
    </tr>
    <tr>
      <td>4.2.7 Usage with limited manipulation or strength</td>
      <td>Partially Supports</td>
      <td>See Section 508 criterion 302.7.</td>
    </tr>
    <tr>
      <td>4.2.8 Usage with limited reach</td>
      <td>Not Applicable</td>
      <td>Web application — no physical reach requirements.</td>
    </tr>
    <tr>
      <td>4.2.9 Minimize photosensitive seizure triggers</td>
      <td>Not Applicable</td>
      <td>See WCAG 2.3.1. Product does not contain flashing content.</td>
    </tr>
    <tr>
      <td>4.2.10 Usage with limited cognition, language or learning</td>
      <td>Partially Supports</td>
      <td>Navigation and error messaging are generally consistent and understandable. Some repeated functions use inconsistent labels, some page titles are generic, and some error messages lack suggested corrections.</td>
    </tr>
    <tr>
      <td>4.2.11 Privacy</td>
      <td>Supports</td>
      <td>Accessibility features provide the same degree of privacy as for non-assistive-technology users. Password fields and assistive technology labels do not expose sensitive information beyond what is visually displayed.</td>
    </tr>
  </tbody>
</table>

### Clause 5: Generic Requirements

Buffer is a web application accessed through standard web browsers. Clause 5 criteria relating to closed functionality (5.1), physical operable parts (5.5), and hardware controls (5.6–5.9) are Not Applicable.

<table>
  <thead>
    <tr>
      <th width="30%" scope="col">Criteria</th>
      <th width="20%" scope="col">Conformance Level</th>
      <th width="50%" scope="col">Remarks and Explanations</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>5.1 Closed functionality</td>
      <td>Not Applicable</td>
      <td>Buffer is not closed-functionality ICT. Users access it through standard browsers with full assistive technology support.</td>
    </tr>
    <tr>
      <td>5.2 Activation of accessibility features</td>
      <td>Supports</td>
      <td>Buffer does not interfere with browser or operating system accessibility features.</td>
    </tr>
    <tr>
      <td>5.3 Biometrics</td>
      <td>Not Applicable</td>
      <td>Product does not use biometric identification.</td>
    </tr>
    <tr>
      <td>5.4 Preservation of accessibility information during conversion</td>
      <td>Partially Supports</td>
      <td>Alt text entered for supported image posts is preserved through publishing to destination platforms. Alt text is not supported for all media formats, and exported analytics PDFs do not preserve semantic structure or chart alternatives.</td>
    </tr>
    <tr>
      <td>5.5–5.9 Operable parts, locking controls, key repeat, double-strike, simultaneous actions</td>
      <td>Not Applicable</td>
      <td>These criteria apply to physical ICT hardware. Buffer is a web application.</td>
    </tr>
  </tbody>
</table>

### Clause 6: ICT with Two-Way Voice Communication

Buffer does not include voice calling, video calling, or real-time text communication features. All Clause 6 criteria are Not Applicable.

### Clause 7: ICT with Video Capabilities

Buffer includes limited feature announcement videos. These are covered in the WCAG media criteria above; other Clause 7 criteria for video communication or hardware are Not Applicable.

### Clause 8: Hardware

Buffer is a web application and does not include hardware components. All Clause 8 criteria are Not Applicable.

### Clause 9: Web

See <a href="#document-top">WCAG 2.x</a> section above. All EN 301 549 Clause 9 criteria map directly to WCAG success criteria.

### Clause 10: Non-Web Documents

Buffer's support documentation is provided as web content. Exported analytics reports are provided as PDFs and are addressed below.

<table>
  <thead>
    <tr>
      <th width="30%" scope="col">Criteria</th>
      <th width="20%" scope="col">Conformance Level</th>
      <th width="50%" scope="col">Remarks and Explanations</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>10.1.1.1 through 10.4.1.3</td>
      <td>Partially Supports</td>
      <td>Support documentation is provided as web content and is addressed in the WCAG section above. Exported analytics PDFs are not tagged and do not preserve reading order or chart alternatives.</td>
    </tr>
    <tr>
      <td>10.5 Caption positioning</td>
      <td>Not Applicable</td>
      <td>Product does not provide non-web documents with captions.</td>
    </tr>
    <tr>
      <td>10.6 Audio description timing</td>
      <td>Not Applicable</td>
      <td>Product does not provide non-web documents with audio description.</td>
    </tr>
  </tbody>
</table>

### Clause 11: Software

EN 301 549 Clause 11 criteria that map to WCAG (11.1.1.1 through 11.4.1.3) are addressed in the WCAG 2.x section above.

<table>
  <thead>
    <tr>
      <th width="30%" scope="col">Criteria</th>
      <th width="20%" scope="col">Conformance Level</th>
      <th width="50%" scope="col">Remarks and Explanations</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>11.1.1.1 through 11.4.1.3</td>
      <td>See <a href="#document-top">WCAG 2.x</a> section</td>
      <td>See information in WCAG 2.x section above.</td>
    </tr>
    <tr>
      <td>11.5 Interoperability with assistive technology</td>
      <td>See <a href="#document-top">WCAG 2.x</a> section</td>
      <td>Buffer is a web application. Assistive technology interoperability is addressed through WCAG criteria, particularly 4.1.2 Name, Role, Value. Platform accessibility services are provided by the browser.</td>
    </tr>
    <tr>
      <td>11.6.1 User control of accessibility features</td>
      <td>Supports</td>
      <td>Buffer does not override or interfere with user-configured accessibility settings.</td>
    </tr>
    <tr>
      <td>11.6.2 No disruption of accessibility features</td>
      <td>Supports</td>
      <td>Buffer does not disrupt browser or OS accessibility features.</td>
    </tr>
    <tr>
      <td>11.7 User preferences</td>
      <td>Supports</td>
      <td>Buffer respects browser and OS user preferences for font size, colors, and motion reduction.</td>
    </tr>
    <tr>
      <td>11.8.2 Accessible content creation</td>
      <td>See <a href="#document-top">WCAG 2.x</a> section</td>
      <td>See also Section 508 criterion 504.2. Alt text input is available for image content where supported by the destination platform.</td>
    </tr>
    <tr>
      <td>11.8.3 Preservation of accessibility information in transformations</td>
      <td>Partially Supports</td>
      <td>Alt text entered for supported image posts is preserved through publishing to destination platforms. Alt text is not supported for all media formats, and exported analytics PDFs do not preserve semantic structure or chart alternatives.</td>
    </tr>
    <tr>
      <td>11.8.4 Repair assistance</td>
      <td>Does Not Support</td>
      <td>Buffer does not help authors identify or repair accessibility issues in authored content. Alt text input is available, but the product does not warn when images lack alt text or prompt authors to fix accessibility issues before publishing.</td>
    </tr>
    <tr>
      <td>11.8.5 Templates</td>
      <td>Not Applicable</td>
      <td>Product does not provide content templates that generate output documents.</td>
    </tr>
  </tbody>
</table>

### Clause 12: Documentation and Support Services

<table>
  <thead>
    <tr>
      <th width="30%" scope="col">Criteria</th>
      <th width="20%" scope="col">Conformance Level</th>
      <th width="50%" scope="col">Remarks and Explanations</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>12.1.1 Accessibility and compatibility features</td>
      <td>Supports</td>
      <td>Accessibility features are documented in the Help Center and in the public Accessibility Statement.</td>
    </tr>
    <tr>
      <td>12.1.2 Accessible documentation</td>
      <td>See <a href="#document-top">WCAG 2.x</a> section</td>
      <td>See information in WCAG 2.x section above.</td>
    </tr>
    <tr>
      <td>12.2.2 Information on accessibility and compatibility features</td>
      <td>Partially Supports</td>
      <td>Buffer does not currently have a dedicated Help Center section covering accessibility features across all product areas.</td>
    </tr>
    <tr>
      <td>12.2.3 Effective communication</td>
      <td>Partially Supports</td>
      <td>Customer support is provided through text-based channels. Known accessibility issues in the chat widget may affect screen reader users.</td>
    </tr>
    <tr>
      <td>12.2.4 Accessible documentation</td>
      <td>See <a href="#document-top">WCAG 2.x</a> section</td>
      <td>See information in WCAG 2.x section above.</td>
    </tr>
  </tbody>
</table>

### Clause 13: ICT Providing Relay or Emergency Service Access

Buffer does not provide relay or emergency services. All Clause 13 criteria are Not Applicable.

---

## Legal Disclaimer

This document is provided for informational purposes and reflects Buffer's self-assessment of accessibility conformance at the time of publication. The information provided does not constitute a warranty or guarantee of accessibility. Buffer is committed to ongoing accessibility improvements.

---

_Report prepared by Buffer — April 2026_

_This VPAT follows the ITI VPAT® 2.5 International Edition format. For questions, contact <a href="mailto:accessibility@buffer.com">accessibility@buffer.com</a>._
