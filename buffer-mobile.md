# <a name="document-top"></a>Buffer Accessibility Conformance Report — Mobile

<b>VPAT® Version 2.5 — International Edition</b>

<b>Name of Product:</b> Buffer

<b>Platform:</b> Mobile Apps (iOS and Android)

<b>Date:</b> September 2026

<b>Contact Information:</b> <a href="mailto:accessibility@buffer.com">accessibility@buffer.com</a>

---

## Status of this report

<b>This report is a work in progress and is published in an incomplete state.</b>

- Buffer's accessibility evaluation of its mobile apps is ongoing. Many success criteria in this report have not yet been formally tested and are recorded as <b>Not Evaluated</b>.
- Testing carried out so far covers the <b>Android app only</b>. The <b>iOS app has not yet been formally evaluated</b> against any criterion in this report.
- Buffer is validating the remaining criteria incrementally and will update this document as results are confirmed. Statuses recorded here may change as evaluation continues.
- We are publishing in this state so that customers and the public can see what has and has not been assessed, rather than waiting for a complete report.

If a specific accessibility criterion matters to your use of Buffer, or you have found an accessibility issue in our mobile apps, please contact <a href="mailto:accessibility@buffer.com">accessibility@buffer.com</a> or open an issue in this repository. We will prioritise evaluating criteria that our customers tell us are important, and <b>we aim to have reported issues fixed within one to two weeks of you reaching out to us</b>.

---

<b>Notes:</b> This report covers accessibility conformance for the Buffer native iOS and Android mobile applications in a single combined document. WCAG success criteria are interpreted for native app context using the W3C <a href="https://www.w3.org/TR/wcag2mobile-22/">WCAG2Mobile</a> guidance. Findings are reported per platform in the Remarks column. Accessibility conformance for the Buffer web application is reported separately in <a href="./buffer-web.md">buffer-web.md</a>.

<b>Evaluation Methods Used:</b> Self-assessment. Manual testing has been carried out on the Android app using TalkBack across a subset of prioritised flows, including primary navigation, the post composer, and calendar and queue views. No formal evaluation of the iOS app has been carried out to date. No automated accessibility scans have been completed for either app; the tooling available for native apps on both platforms (iOS Accessibility Inspector and Android Accessibility Scanner) requires manual, per-screen operation rather than a full automated audit, and results from these tools are not yet reflected in this report.

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
  <li><b>Not Evaluated:</b> The product has not yet been tested against the criterion. In this report, Not Evaluated is used extensively — see <a href="#document-top">Status of this report</a> above.</li>
</ul>

<b>How iOS and Android are reported together:</b> This report covers both mobile apps in a single set of tables. The Conformance Level column records one combined status for both platforms, applied conservatively:

<ul>
  <li>Where a defect has been identified on either platform, the combined status reflects that defect.</li>
  <li>Where a criterion has been tested and passed on one platform but not yet tested on the other, the combined status is <b>Not Evaluated</b> and the passing result is described in the Remarks. A combined status will be recorded once both platforms have been tested.</li>
  <li>Where neither platform has been tested, the combined status is <b>Not Evaluated</b>.</li>
</ul>

Platform-specific detail is given in the Remarks column, prefixed with <b>iOS:</b>, <b>Android:</b>, or <b>Both platforms:</b>.

---

## <a name="wcag-2-x"></a>WCAG 2.x Report

The WCAG criteria below are applicable to the following standards:

- EN 301 549: Clause 11 (Software), which covers native mobile applications
- Revised Section 508: Chapter 5 — 501.1 Scope

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
      <td><b>Android:</b> Most icons, buttons, and other elements announce meaningful information in the flows tested. The Instagram hashtag count control does not announce meaningful text. <b>iOS:</b> Not evaluated.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#audio-only-and-video-only-prerecorded">1.2.1 Audio-only and Video-only (Prerecorded)</a> (Level A)</td>
      <td>Not Applicable</td>
      <td><b>Both platforms:</b> The mobile apps do not present prerecorded audio-only or video-only content.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#captions-prerecorded">1.2.2 Captions (Prerecorded)</a> (Level A)</td>
      <td>Not Applicable</td>
      <td><b>Both platforms:</b> The mobile apps do not include in-app video content.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#audio-description-or-media-alternative-prerecorded">1.2.3 Audio Description or Media Alternative (Prerecorded)</a> (Level A)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated. The mobile apps are not understood to include prerecorded media content (see 1.2.1 and 1.2.2); this will be confirmed in a future review.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#info-and-relationships">1.3.1 Info and Relationships</a> (Level A)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#meaningful-sequence">1.3.2 Meaningful Sequence</a> (Level A)</td>
      <td>Not Evaluated</td>
      <td><b>Android:</b> Reading order followed the visual order in the flows tested with TalkBack; no defects were identified. <b>iOS:</b> Not evaluated. A combined conformance level will be recorded once iOS has been tested.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#sensory-characteristics">1.3.3 Sensory Characteristics</a> (Level A)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#use-of-color">1.4.1 Use of Color</a> (Level A)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#audio-control">1.4.2 Audio Control</a> (Level A)</td>
      <td>Not Applicable</td>
      <td><b>Both platforms:</b> No audio plays automatically in the mobile apps.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#keyboard">2.1.1 Keyboard</a> (Level A)</td>
      <td>Not Evaluated</td>
      <td>For native apps this criterion covers external keyboard input and platform switch control (Switch Control on iOS, Switch Access on Android). Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#no-keyboard-trap">2.1.2 No Keyboard Trap</a> (Level A)</td>
      <td>Partially Supports</td>
      <td><b>Android:</b> Focus could be moved away from all components in the flows tested, except when exiting the composer, where focus could not be moved away. <b>iOS:</b> Not evaluated.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#character-key-shortcuts">2.1.4 Character Key Shortcuts</a> (Level A — WCAG 2.1)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#timing-adjustable">2.2.1 Timing Adjustable</a> (Level A)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#pause-stop-hide">2.2.2 Pause, Stop, Hide</a> (Level A)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#three-flashes-or-below-threshold">2.3.1 Three Flashes or Below Threshold</a> (Level A)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#bypass-blocks">2.4.1 Bypass Blocks</a> (Level A)</td>
      <td>Not Applicable</td>
      <td><b>Both platforms:</b> Native apps do not present repeated blocks of content that require a skip mechanism in the web sense. The equivalent function is provided by the platform screen reader through the VoiceOver rotor and TalkBack reading controls.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#page-titled">2.4.2 Page Titled</a> (Level A)</td>
      <td>Partially Supports</td>
      <td>Applied to mobile as screen titles. <b>Android:</b> Screen names are announced when moving between screens, with focus starting on the back control. The Create screen does not announce a title on entry; users have to navigate to the tab bar to identify the section. <b>iOS:</b> Not evaluated.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#focus-order">2.4.3 Focus Order</a> (Level A)</td>
      <td>Partially Supports</td>
      <td><b>Android:</b> Focus moved in a logical order across the flows tested, except when exiting the composer, where focus was trapped. <b>iOS:</b> Not evaluated.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#link-purpose-in-context">2.4.4 Link Purpose (In Context)</a> (Level A)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#pointer-gestures">2.5.1 Pointer Gestures</a> (Level A — WCAG 2.1)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#pointer-cancellation">2.5.2 Pointer Cancellation</a> (Level A — WCAG 2.1)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#label-in-name">2.5.3 Label in Name</a> (Level A — WCAG 2.1)</td>
      <td>Partially Supports</td>
      <td><b>Android:</b> Most icon-only controls and other elements announce a name that matches their visible purpose. The Instagram hashtag count control does not announce meaningful text, and calendar day headings are announced as single letters (for example, "M") rather than the full day name. <b>iOS:</b> Not evaluated.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#motion-actuation">2.5.4 Motion Actuation</a> (Level A — WCAG 2.1)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#language-of-page">3.1.1 Language of Page</a> (Level A)</td>
      <td>Not Evaluated</td>
      <td>Applied to mobile as the declared app language. Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#on-focus">3.2.1 On Focus</a> (Level A)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#on-input">3.2.2 On Input</a> (Level A)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG22/#consistent-help">3.2.6 Consistent Help</a> (Level A — WCAG 2.2)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#error-identification">3.3.1 Error Identification</a> (Level A)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#labels-or-instructions">3.3.2 Labels or Instructions</a> (Level A)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG22/#redundant-entry">3.3.7 Redundant Entry</a> (Level A — WCAG 2.2)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#parsing">4.1.1 Parsing</a> (Level A)</td>
      <td>Not Applicable</td>
      <td><b>Both platforms:</b> Obsoleted in WCAG 2.2 and automatically satisfied per W3C guidance. Native apps do not use HTML parsing.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#name-role-value">4.1.2 Name, Role, Value</a> (Level A)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform. Related label findings are recorded under 1.1.1 and 2.5.3.</td>
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
      <td><b>Both platforms:</b> The mobile apps do not include live audio or video content.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#audio-description-prerecorded">1.2.5 Audio Description (Prerecorded)</a> (Level AA)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated. The mobile apps are not understood to include prerecorded media content (see 1.2.1 and 1.2.2); this will be confirmed in a future review.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#orientation">1.3.4 Orientation</a> (Level AA — WCAG 2.1)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#identify-input-purpose">1.3.5 Identify Input Purpose</a> (Level AA — WCAG 2.1)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#contrast-minimum">1.4.3 Contrast (Minimum)</a> (Level AA)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#resize-text">1.4.4 Resize Text</a> (Level AA)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#images-of-text">1.4.5 Images of Text</a> (Level AA)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#reflow">1.4.10 Reflow</a> (Level AA — WCAG 2.1)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#non-text-contrast">1.4.11 Non-text Contrast</a> (Level AA — WCAG 2.1)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#text-spacing">1.4.12 Text Spacing</a> (Level AA — WCAG 2.1)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#content-on-hover-or-focus">1.4.13 Content on Hover or Focus</a> (Level AA — WCAG 2.1)</td>
      <td>Not Applicable</td>
      <td><b>Both platforms:</b> The mobile apps do not present content on hover or focus. Native mobile touch interfaces do not provide a hover state.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#multiple-ways">2.4.5 Multiple Ways</a> (Level AA)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#headings-and-labels">2.4.6 Headings and Labels</a> (Level AA)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#focus-visible">2.4.7 Focus Visible</a> (Level AA)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG22/#focus-not-obscured-minimum">2.4.11 Focus Not Obscured (Minimum)</a> (Level AA — WCAG 2.2)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG22/#dragging-movements">2.5.7 Dragging Movements</a> (Level AA — WCAG 2.2)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG22/#target-size-minimum">2.5.8 Target Size (Minimum)</a> (Level AA — WCAG 2.2)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#language-of-parts">3.1.2 Language of Parts</a> (Level AA)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#consistent-navigation">3.2.3 Consistent Navigation</a> (Level AA)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#consistent-identification">3.2.4 Consistent Identification</a> (Level AA)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#error-suggestion">3.3.3 Error Suggestion</a> (Level AA)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#error-prevention-legal-financial-data">3.3.4 Error Prevention (Legal, Financial, Data)</a> (Level AA)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG22/#accessible-authentication-minimum">3.3.8 Accessible Authentication (Minimum)</a> (Level AA — WCAG 2.2)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#status-messages">4.1.3 Status Messages</a> (Level AA — WCAG 2.1)</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
  </tbody>
</table>

### Table 3: Success Criteria, Level AAA

This report does not include Level AAA criteria. Buffer is reporting against WCAG 2.2 Levels A and AA, including WCAG 2.1 Level AA criteria.

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
      <td><b>Android:</b> Screen reader testing of a subset of prioritised flows found that most elements announce meaningful information and that reading order followed visual order, but also identified defects that affect use without vision: a focus trap when exiting the composer, a missing screen title on the Create screen, and controls that do not announce meaningful text (see 1.1.1, 2.1.2, 2.4.2, 2.4.3, and 2.5.3). <b>iOS:</b> Not evaluated.</td>
    </tr>
    <tr>
      <td>302.2 With Limited Vision</td>
      <td>Not Evaluated</td>
      <td>Text scaling, contrast, and platform display settings have not yet been formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td>302.3 Without Perception of Color</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td>302.4 Without Hearing</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated. The mobile apps are not understood to rely on audio for any workflow (see 1.2.1 and 1.4.2); this will be confirmed in a future review.</td>
    </tr>
    <tr>
      <td>302.5 With Limited Hearing</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated. The mobile apps are not understood to rely on audio for any workflow (see 1.2.1 and 1.4.2); this will be confirmed in a future review.</td>
    </tr>
    <tr>
      <td>302.6 Without Speech</td>
      <td>Not Applicable</td>
      <td><b>Both platforms:</b> No feature in the mobile apps requires speech input.</td>
    </tr>
    <tr>
      <td>302.7 With Limited Manipulation</td>
      <td>Not Evaluated</td>
      <td>Switch control, assistive touch, and external input have not yet been formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td>302.8 With Limited Reach and Strength</td>
      <td>Not Applicable</td>
      <td><b>Both platforms:</b> Buffer provides software applications that run on standard consumer smartphones. Buffer does not provide hardware requiring reach or strength.</td>
    </tr>
    <tr>
      <td>302.9 With Limited Language, Cognitive, and Learning Abilities</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
  </tbody>
</table>

### Chapter 4: Hardware

Buffer provides mobile applications that run on standard consumer smartphones. Buffer does not provide hardware components. All Chapter 4 criteria are Not Applicable.

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
      <td>See <a href="#wcag-2-x">WCAG 2.x</a> section</td>
      <td>See information in WCAG 2.x section above.</td>
    </tr>
    <tr>
      <td>502 Interoperability with Assistive Technology</td>
      <td>See <a href="#wcag-2-x">WCAG 2.x</a> section</td>
      <td>Assistive technology interoperability for native apps is addressed through the WCAG criteria above, particularly 1.1.1, 2.5.3, and 4.1.2. Known gaps identified on Android are recorded in those rows. iOS has not been evaluated.</td>
    </tr>
    <tr>
      <td>503.2 User Preferences</td>
      <td>Not Evaluated</td>
      <td>The apps' handling of platform accessibility preferences — including text size, bold text, reduced motion, increased contrast, and colour filters — has not yet been formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td>503.3 Alternative User Interfaces</td>
      <td>Not Applicable</td>
      <td><b>Both platforms:</b> The mobile apps do not provide alternative user interfaces.</td>
    </tr>
    <tr>
      <td>503.4 User Controls for Captions and Audio Description</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated. The mobile apps are not understood to include an in-app video player (see 1.2.2); this will be confirmed in a future review.</td>
    </tr>
    <tr>
      <td>504.2 Content Creation or Editing</td>
      <td>Not Evaluated</td>
      <td>Buffer is an authoring tool for social media content. Whether alt text can be entered in the mobile composer, and for which media types, has not yet been formally evaluated.</td>
    </tr>
    <tr>
      <td>504.2.1 Preservation of Information in Format Conversion</td>
      <td>Not Evaluated</td>
      <td>Whether alt text entered in the mobile apps is preserved through publishing to destination platforms has not yet been formally evaluated.</td>
    </tr>
    <tr>
      <td>504.2.2 PDF Export</td>
      <td>Not Applicable</td>
      <td><b>Both platforms:</b> The mobile apps do not export PDFs.</td>
    </tr>
    <tr>
      <td>504.3 Prompts</td>
      <td>Not Evaluated</td>
      <td>Whether the mobile composer prompts or warns authors when images are published without alt text has not yet been formally evaluated.</td>
    </tr>
    <tr>
      <td>504.4 Templates</td>
      <td>Not Applicable</td>
      <td><b>Both platforms:</b> The mobile apps do not provide document templates.</td>
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
      <td>Not Evaluated</td>
      <td>Whether Buffer's Help Center and <a href="https://buffer.com/accessibility">accessibility statement</a> document mobile-specific accessibility features has not yet been formally reviewed.</td>
    </tr>
    <tr>
      <td>602.3 Electronic Support Documentation</td>
      <td>See <a href="./buffer-web.md">web report</a></td>
      <td>Buffer's support documentation is delivered as web content and is covered by the Buffer web Accessibility Conformance Report.</td>
    </tr>
    <tr>
      <td>602.4 Alternate Formats for Non-Electronic Support Documentation</td>
      <td>Not Applicable</td>
      <td>All support documentation is provided electronically.</td>
    </tr>
    <tr>
      <td>603.2 Information on Accessibility and Compatibility Features</td>
      <td>Not Evaluated</td>
      <td>Support services are shared across web and mobile. Mobile-specific coverage has not yet been formally reviewed.</td>
    </tr>
    <tr>
      <td>603.3 Accommodation of Communication Needs</td>
      <td>Not Evaluated</td>
      <td>Access to support from within the mobile apps has not yet been formally evaluated with VoiceOver or TalkBack.</td>
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
      <td>Not Evaluated</td>
      <td>See Section 508 criterion 302.2.</td>
    </tr>
    <tr>
      <td>4.2.3 Usage without perception of colour</td>
      <td>Not Evaluated</td>
      <td>See Section 508 criterion 302.3.</td>
    </tr>
    <tr>
      <td>4.2.4 Usage without hearing</td>
      <td>Not Evaluated</td>
      <td>See Section 508 criterion 302.4.</td>
    </tr>
    <tr>
      <td>4.2.5 Usage with limited hearing</td>
      <td>Not Evaluated</td>
      <td>See Section 508 criterion 302.5.</td>
    </tr>
    <tr>
      <td>4.2.6 Usage with no or limited vocal capability</td>
      <td>Not Applicable</td>
      <td><b>Both platforms:</b> No feature in the mobile apps requires speech input.</td>
    </tr>
    <tr>
      <td>4.2.7 Usage with limited manipulation or strength</td>
      <td>Not Evaluated</td>
      <td>See Section 508 criterion 302.7.</td>
    </tr>
    <tr>
      <td>4.2.8 Usage with limited reach</td>
      <td>Not Applicable</td>
      <td><b>Both platforms:</b> Buffer does not provide hardware.</td>
    </tr>
    <tr>
      <td>4.2.9 Minimize photosensitive seizure triggers</td>
      <td>Not Evaluated</td>
      <td>See WCAG 2.3.1.</td>
    </tr>
    <tr>
      <td>4.2.10 Usage with limited cognition, language or learning</td>
      <td>Not Evaluated</td>
      <td>See Section 508 criterion 302.9.</td>
    </tr>
    <tr>
      <td>4.2.11 Privacy</td>
      <td>Not Evaluated</td>
      <td>Whether the mobile apps expose sensitive information to assistive technology beyond what is visually displayed — including password field behaviour with VoiceOver and TalkBack — has not yet been formally evaluated.</td>
    </tr>
  </tbody>
</table>

### Clause 5: Generic Requirements

Most Clause 5 criteria relate to hardware or closed functionality and are Not Applicable to the Buffer mobile apps.

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
      <td>The mobile apps run on general-purpose smartphones with full access to the operating system's assistive technologies.</td>
    </tr>
    <tr>
      <td>5.2 Activation of accessibility features</td>
      <td>Not Evaluated</td>
      <td>Whether the mobile apps interfere with platform accessibility features has not yet been formally evaluated.</td>
    </tr>
    <tr>
      <td>5.3 Biometrics</td>
      <td>Not Evaluated</td>
      <td>Whether the mobile apps offer biometric authentication, and whether a non-biometric alternative is available, has not yet been formally evaluated.</td>
    </tr>
    <tr>
      <td>5.4 Preservation of accessibility information during conversion</td>
      <td>Not Evaluated</td>
      <td>See Section 508 criterion 504.2.1.</td>
    </tr>
    <tr>
      <td>5.5–5.9 Operable parts, locking controls, key repeat, double-strike, simultaneous actions</td>
      <td>Not Applicable</td>
      <td>These criteria apply to physical ICT hardware. Buffer provides software applications only.</td>
    </tr>
  </tbody>
</table>

### Clause 6: ICT with Two-Way Voice Communication

The Buffer mobile apps do not include voice calling, video calling, or real-time text communication features. All Clause 6 criteria are Not Applicable.

### Clause 7: ICT with Video Capabilities

The Buffer mobile apps do not provide video communication capabilities. All Clause 7 criteria are Not Applicable. Media handling in the composer is covered by the WCAG criteria above.

### Clause 8: Hardware

Buffer does not provide hardware components. All Clause 8 criteria are Not Applicable.

### Clause 9: Web

Not Applicable to this report. Conformance for Buffer's web application is reported separately in <a href="./buffer-web.md">buffer-web.md</a>.

### Clause 10: Non-Web Documents

Not Applicable. The Buffer mobile apps do not create or export non-web documents.

### Clause 11: Software

Clause 11 is the relevant EN 301 549 clause for native mobile applications. Criteria 11.1.1.1 through 11.4.1.3 map to WCAG success criteria and are addressed in the WCAG 2.x section above.

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
      <td>See <a href="#wcag-2-x">WCAG 2.x</a> section</td>
      <td>See information in WCAG 2.x section above.</td>
    </tr>
    <tr>
      <td>11.5 Interoperability with assistive technology</td>
      <td>See <a href="#wcag-2-x">WCAG 2.x</a> section</td>
      <td>See Section 508 criterion 502. Interoperability is addressed through the WCAG criteria above, particularly 1.1.1, 2.5.3, and 4.1.2.</td>
    </tr>
    <tr>
      <td>11.6.1 User control of accessibility features</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td>11.6.2 No disruption of accessibility features</td>
      <td>Not Evaluated</td>
      <td>Not yet formally evaluated on either platform.</td>
    </tr>
    <tr>
      <td>11.7 User preferences</td>
      <td>Not Evaluated</td>
      <td>See Section 508 criterion 503.2.</td>
    </tr>
    <tr>
      <td>11.8.2 Accessible content creation</td>
      <td>Not Evaluated</td>
      <td>See Section 508 criterion 504.2.</td>
    </tr>
    <tr>
      <td>11.8.3 Preservation of accessibility information in transformations</td>
      <td>Not Evaluated</td>
      <td>See Section 508 criterion 504.2.1.</td>
    </tr>
    <tr>
      <td>11.8.4 Repair assistance</td>
      <td>Not Evaluated</td>
      <td>See Section 508 criterion 504.3.</td>
    </tr>
    <tr>
      <td>11.8.5 Templates</td>
      <td>Not Applicable</td>
      <td><b>Both platforms:</b> The mobile apps do not provide content templates that generate output documents.</td>
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
      <td>Not Evaluated</td>
      <td>See Section 508 criterion 602.2.</td>
    </tr>
    <tr>
      <td>12.1.2 Accessible documentation</td>
      <td>See <a href="./buffer-web.md">web report</a></td>
      <td>Support documentation is delivered as web content and is covered by the Buffer web Accessibility Conformance Report.</td>
    </tr>
    <tr>
      <td>12.2.2 Information on accessibility and compatibility features</td>
      <td>Not Evaluated</td>
      <td>See Section 508 criterion 603.2.</td>
    </tr>
    <tr>
      <td>12.2.3 Effective communication</td>
      <td>Not Evaluated</td>
      <td>See Section 508 criterion 603.3.</td>
    </tr>
    <tr>
      <td>12.2.4 Accessible documentation</td>
      <td>See <a href="./buffer-web.md">web report</a></td>
      <td>Support documentation is delivered as web content and is covered by the Buffer web Accessibility Conformance Report.</td>
    </tr>
  </tbody>
</table>

### Clause 13: ICT Providing Relay or Emergency Service Access

Buffer does not provide relay or emergency services. All Clause 13 criteria are Not Applicable.

---

## Legal Disclaimer

This document is provided for informational purposes and reflects Buffer's self-assessment of the accessibility of its mobile applications at the time of publication. Evaluation is incomplete: many criteria are recorded as Not Evaluated, and the iOS app has not yet been formally tested. The information provided does not constitute a warranty or guarantee of accessibility. Buffer is committed to ongoing accessibility improvements and to updating this report as evaluation progresses.

---

_Report prepared by Buffer — September 2026_

_This VPAT follows the ITI VPAT® 2.5 International Edition format. For questions, contact <a href="mailto:accessibility@buffer.com">accessibility@buffer.com</a>._
