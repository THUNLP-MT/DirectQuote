# DirectQuote - A Dataset for Direct Quotation Extraction and Attribution in News Articles

DirectQuote is a corpus containing 19,760 paragraphs and 10,353 direct quotations manually annotated from online news media.

A _quotation_ is a general notion that covers different kinds of speech, thought, and writing in text (Semino and Short,2004). It is a prominent linguistic device for expressing opinions, statements, and assessments attributed to the speaker (Cappelen and Lepore, 2012). Among all kinds of quotations, the entire content of the _direct quotation_ (O’Keefe et al.,2013) is in quotation marks, which means that what the speaker said is transcribed verbatim.

## Task Definition
Quotation extractionis defined as extracting reported speech from a third party in the text, also known as reportedspeech extraction. Quotation attribution refers to determining the speaker of the quotation. When annotating speakers, we ensure that valid speakers should be able to belinked to a person entity in a named entity library. Among them, simple patterns are removed to increase the diversity of the corpus. 

## Data 


<table>
   <tr>
      <td>Region</td>
      <td>Name</td>
      <td>Numbers</td>
   </tr>
   <tr>
      <td rowspan="5">U.S.</td>
      <td>Associated Press</td>
      <td>438</td>
   </tr>
   <tr>
      <td>Cable News Network</td>
      <td>627</td>
   </tr>
   <tr>
      <td>American Broadcasting Company</td>
      <td>240</td>
   </tr>
   <tr>
      <td>New York Times</td>
      <td>5,642</td>
   </tr>
   <tr>
      <td>CBS Broadcasting</td>
      <td>4,890</td>
   </tr>
   <tr>
      <td rowspan="3">UK</td>
      <td>British Broadcasting Corporation</td>
      <td>926</td>
   </tr>
   <tr>
      <td>Reuters</td>
      <td>5,836</td>
   </tr>
   <tr>
      <td>The Guardian</td>
      <td>4,302</td>
   </tr>
   <tr>
      <td rowspan="2">Canada</td>
      <td>The Globe and Mail</td>
      <td>1,955</td>
   </tr>
   <tr>
      <td>The Star</td>
      <td>13,769</td>
   </tr>
   <tr>
      <td>New Zealand</td>
      <td>NZ Herald</td>
      <td>115</td>
   </tr>
   <tr>
      <td rowspan="2">Australia</td>
      <td>Australian Broadcasting Corporation</td>
      <td>312</td>
   </tr>
   <tr>
      <td>Sydney Morning Herald</td>
      <td>93</td>
   </tr>
</table>

We select representative and multiple news sources across the political spectrum, including 13 well-known online news media from five major English-speaking countries. The corpus adopts the format consistent with CoNLL 2003. We use IOB1 format in the corpus. Raw texts are tokenized by whitespace tokenizer. Every word is classified into the following lables:

* `LeftSpeaker` Quotation, the corresponding speaker is in the preceding text
* `RightSpeaker` Quotation, the corresponding speaker is in the following text
* `Unknown` Quotation, no corresponding speaker
* `Speaker` Speaker
* `Out` Neither


## Statistics
|              | Numbers         |
| ------------ | --------------- |
| News Article | 39,153          |
| Paragraph    | 19,760          |
| Quotation    | 10,353          |
| Time         | 2020.09-2021.03 |


## Reference
_DirectQuote: A Dataset for Direct Quotation Extraction and Attribution in News Articles_, Yuanchi Zhang, Yang Liu