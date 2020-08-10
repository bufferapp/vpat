
# <a name="document-top"></a>Buffer Voluntary Product Accessibility Template (VPAT)

<b>VPAT® Version 2.1</b>

<b>Name of Product:</b> Buffer

<b>Platform:</b> Web

<b>Date:</b> August 2020

<b>Contact Information:</b> <a href = "mailto: accessibility@buffer.com">accessibility@buffer.com</a>

<b>Notes:</b> This report covers accessibility conformance for the Buffer product which includes the product suite Publish, Analyze and Engage.

<b>Evaluation Methods Used:</b> Conformance to the listed accessibility standards has been done through self-evaluation.

## Terms
The terms used in the Conformance Level information are defined as follows:

<ul>
	<li><b>Supports:</b> The functionality of the product has at least one method that meets the criterion without known defects or meets with equivalent facilitation.</li>
	<li><b>Supports with Exceptions:</b> Some functionality of the product does not meet the criterion.</li>
	<li><b>Does Not Support:</b> The majority of product functionality does not meet the criterion.</li>
	<li><b>Not Applicable:</b> The criterion is not relevant to the product.</li>
	<li><b>Not Evaluated:</b> The product has not been evaluated against the criterion. This can be used only in WCAG 2.0 Level AAA.</li>
</ul>

## Table 1: Success Criteria, Level A

<table>
  <thead>
    <tr>
      <th width="30%" scope="col">Criteria</th>
      <th width="20%" scope="col">Conformance Level</th>
      <th width="50%" scope="col">Remarks and explanations</th>
    </tr>
	</thead>
	<tbody>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#text-equiv-all">1.1.1 Non-text Content (Level A)</a></td>
      <td>Supports with exceptions</td>
      <td>
        <ul>
          <li>Analyze and Engage makes use of icons with no text (for downloading invoices). </li>
          <li>Images and graphs related to posts in Analyze do not have text. </li>
          <li>Some non-text post content in Publish does not have text associated with it.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#media-equiv-av-only-alt">1.2.1 Audio-only and Video-only (Prerecorded) (Level A)</a></td>
      <td>Not applicable</td>
      <td></td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#media-equiv-captions"> 1.2.2 Captions (Prerecorded) (Level A)</a></td>
      <td>Supports</td>
      <td>
				<ul>
					<li>Informational videos are hosted on YouTube with automatic captioning.</li>
				</ul>
			</td>
    </tr>
    <tr>
      <td>
        <a href="http://www.w3.org/TR/WCAG20/#media-equiv-audio-desc">1.2.3 Audio Description or Media Alternative (Prerecorded) (Level A)</a>
      </td>
      <td>Not applicable</td>
      <td></td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#content-structure-separation-programmatic">1.3.1 Info and Relationships (Level A)</a></td>
      <td>Supports with exceptions</td>
      <td>
        <ul>
          <li> A few tables may not be using the table element.</li>
          <li>Buffer strives for semantically-correct markup though we’re still working to make it 100%.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#content-structure-separation-sequence">1.3.2 Meaningful Sequence (Level A)</a></td>
      <td>Supports</td>
      <td>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#content-structure-separation-understanding">1.3.3 Sensory Characteristics  (Level A)</a></td>
      <td>Supports with exceptions</td>
      <td>
        <ul>
          <li>Engage labels do not have a text element, just an icon + tooltip.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#visual-audio-contrast-without-color">1.4.1 Use of Color (Level A)</a></td>
      <td>Supports</td>
      <td>
        <ul>
          <li>Engage uses labels with different colors associated and the only way of differentiating them is to rely on the displayed icon or tooltip.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#visual-audio-contrast-dis-audio">1.4.2 Audio Control (Level A)</a></td>
      <td>Supports</td>
      <td>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#keyboard-operation-keyboard-operable">2.1.1 Keyboard (Level A)</a></td>
      <td>Supports with exceptions</td>
      <td>
        <ul>
          <li>Engage and billing sidebar cannot be navigated with the keyboard. </li>
          <li>Engage channel selector cannot be accessed with the keyboard.</li>
          <li>Changing plans within the modal in billing is not accessible with keyboard.</li>
          <li>Though Buffer routinely identifies and fixes keyboard accessibility issues across the applications, it is possible that there are still some issues with keyboard compatibility. Buffer strives to assess and fix any keyboard compatibility issues found internally or externally as promptly as possible.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#keyboard-operation-trapping">2.1.2 No Keyboard Trap (Level A)</a></td>
      <td>Supports with exceptions</td>
      <td>
        <ul>
          <li>The Publish composer does not have a way to escape the modal through keyboard or escape key. </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#time-limits-required-behaviors">2.2.1 Timing Adjustable (Level A)</a></td>
      <td>Not applicable</td>
      <td>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#time-limits-pause">2.2.2 Pause, Stop, Hide (Level A)</a></td>
      <td>Not applicable</td>
      <td>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#seizure-does-not-violate">2.3.1 Three Flashes or Below Threshold (Level A)</a></td>
      <td>Supports with exceptions</td>
      <td>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#navigation-mechanisms-skip">2.4.1 Bypass Blocks (Level A)</a></td>
      <td>Supports with exceptions</td>
      <td>
        <ul>
          <li>Publish currently has a skip to main content screen reader accessible link before the navbar.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#navigation-mechanisms-title">2.4.2 Page Titled (Level A)</a></td>
      <td>Supports</td>
      <td>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#navigation-mechanisms-focus-order">2.4.3 Focus Order (Level A)</a></td>
      <td>Supports with exceptions</td>
      <td>
        <ul>
          <li>Engage focus does not work properly with the sidebar post grid.</li>
          <li>Publish has parts of the composer where the focus order is incorrect.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#navigation-mechanisms-refs">2.4.4 Link Purpose (In Context) (Level A)</a></td>
      <td>Supports with exceptions</td>
      <td>
        <ul>
          <li>Analyze download invoice button and reconnect and remove social account buttons are an icon without any text. </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#meaning-doc-lang-id">3.1.1 Language of Page (Level A)</a></td>
      <td>Supports</td>
      <td>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#consistent-behavior-receive-focus">3.2.1 On Focus (Level A)</a></td>
      <td>Supports</td>
      <td>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#consistent-behavior-unpredictable-change">3.2.2 On Input (Level A)</a></td>
      <td>Supports with exceptions</td>
      <td>
        <ul>
          <li>In an Engage comment reply, hitting “Enter” will cause the reply to be sent and the focus will be moved to the next unprocessed comment on the list.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#minimize-error-identified">3.3.1 Error Identification (Level A)</a></td>
      <td>Supports with exceptions</td>
      <td>
        <ul>
          <li>When creating Analyze reports, a user is not notified if the module fails to be added to the report.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#minimize-error-cues">3.3.2 Labels or Instructions (Level A)</a></td>
      <td>Supports with exceptions</td>
      <td>
        <ul>
          <li>There may be some cases where labels are missing or missing relationship with fields.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#ensure-compat-parses">4.1.1 Parsing (Level A)</a></td>
      <td>Supports with exceptions</td>
      <td>
        <ul>
          <li>Some pages feature inputs with non-unique ids.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#ensure-compat-rsv">4.1.2 Name, Role, Value (Level A)</a></td>
      <td>Supports with exceptions</td>
      <td>
        <ul>
          <li>A majority of information about user interface elements provide sufficient information about the identity, operation and state of the elements. Buffer is still working to make sure the application has 100% coverage of accessible user interface elements.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## Table 2: Success Criteria, Level AA

<table>
  <thead>
    <tr>
      <th width="30%">Criteria</th>
      <th width="20%">Conformance Level</th>
      <th width="50%">Remarks and explanations</th>
    </tr>
	</thead>
	<tbody>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#media-equiv-audio-desc-only">1.2.4 Captions (Live) (Level AA)</a></td>
      <td>Not applicable</td>
      <td>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#media-equiv-av-only-alt">1.2.5 Audio Description (Prerecorded) (Level AA)</a></td>
      <td>Not applicable</td>
      <td>
        <ul>
          <li>Audio descriptions are not required for information retrieval in Buffer informational videos.
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#orientation"> 1.3.4 Orientation (Level AA 2.1 only)</a></td>
      <td> Supports with exceptions</td>
      <td>
        <ul>
          <li>Analyze is a web app meant to be used on computer screens in a horizontal orientation.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>
        <a href="https://www.w3.org/TR/WCAG21/#identify-input-purpose">1.3.5 Identify Input Purpose (Level AA 2.1 only)</a>
      </td>
      <td>Supports with exceptions</td>
      <td>        
        <ul>
          <li>Buffer sets type on inputs for password, but not for updating a user’s email address.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#visual-audio-contrast-contrast">1.4.3 Contrast (Minimum) (Level AA)</a></td>
      <td>Supports with exceptions</td>
      <td>
        <ul>
          <li>Buffer strives to display readable, contrasted text, however there may be cases where the text contrast does not meet the minimum requirements.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#content-structure-separation-sequence">1.4.4 Resize text (Level AA)</a></td>
      <td>Supports with exceptions</td>
      <td>
        <ul>
          <li>Analyze content carousels break past 150%.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#visual-audio-contrast-text-presentation">1.4.5 Images of Text (Level AA)</a></td>
      <td>Supports</td>
      <td>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#visual-audio-contrast-without-color">1.4.10 Reflow (Level AA 2.1 only)</a></td>
      <td>Not supported</td>
      <td>
        <ul>
          <li>Publish supports content magnified up to 400% without the need to scroll in more than one direction to perform primary tasks. The user may need to scroll in more than one direction to access all of the content in Publish at 400% magnification.</li>
          <li>Engage and Analyze are non-responsive.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#visual-audio-contrast-dis-audio">1.4.11 Non-text Contrast (Level AA 2.1 only)</a></td>
      <td>Supports with exceptions</td>
      <td>
        <ul>
          <li>While the majority of elements meet contrast, there may be some cases where the non-text contrast does not meet the minimum requirements.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#text-spacing">1.4.12 Text Spacing (Level AA 2.1 only)</a></td>
      <td>Supports</td>
      <td>
      </td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#content-on-hover-or-focus">1.4.13 Content on Hover or Focus (Level AA 2.1 only)</a></td>
      <td>Not supported</td>
      <td>
        <ul>
          <li>Buffer tooltips are not dismissable.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#navigation-mechanisms-descriptive">2.4.5 Multiple Ways (Level AA)</a></td>
      <td>Supports with exceptions</td>
      <td>
        <ul>
          <li>Engage does not display any headings and is missing labels.</li>
          <li>Account pages have missing required fields and properties with some labels.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#time-limits-pause">2.4.6 Headings and Labels (Level AA)</a></td>
      <td>Supports with exceptions</td>
      <td>
        <ul>
          <li>Engage does not display any headings and is missing labels.</li>
          <li>Account pages have missing required fields and properties with some labels.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#navigation-mechanisms-focus-visible">2.4.7 Focus Visible (Level AA)</a></td>
      <td>Supports with exceptions</td>
      <td>
        <ul>
          <li>Publish and Analyze have a few exceptions where a focus indicator is not present.</li>
          <li>Analyze does not have a focus indicator with channel sidebar and tabs.</li>
        <ul>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#meaning-other-lang-id">3.1.2 Language of Parts (Level AA)</a></td>
      <td>Not applicable</td>
      <td>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#consistent-behavior-consistent-locations">3.2.3 Consistent Navigation (Level AA)</a></td>
      <td>Supports</td>
      <td>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#consistent-behavior-consistent-functionality">3.2.4 Consistent Identification (Level AA)</a></td>
      <td>Supports</td>
      <td>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#minimize-error-suggestions">3.3.3 Error Suggestion (Level AA)</a></td>
      <td>Supports with exceptions</td>
      <td>
        <ul>
          <li>In Engage, if a user tries to send an empty reply, no error will display.</li>
          <li>In billing, credit card related errors from Stripe use a generic error message.</li>
          <li>Analyze is missing specific post insights and report errors.</li>
          <li>Publish has error messages that are not accessible with a screen reader.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#minimize-error-reversible">3.3.4 Error Prevention (Legal, Financial, Data) (Level AA)</a></td>
      <td>Not applicable</td>
      <td>
      </td>
    </tr>
    <tr>
      <td><a href="https://www.w3.org/TR/WCAG21/#status-messages">4.1.3 Status Messages (Level AA 2.1 only)</a></td>
      <td>Supports</td>
      <td>
      </td>
    </tr>
    <tr>
      <td><a href="http://www.w3.org/TR/WCAG20/#consistent-behavior-unpredictable-change">3.2.2 On Input (Level A)</a></td>
      <td>Supports with exceptions</td>
      <td>
        <ul>
          <li>Engage role properties are missing on elements displaying status information.</li>
          <li>Publish and Analyze have notifications that are not announced to screen readers.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


