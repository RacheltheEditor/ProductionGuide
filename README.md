# Production Guide

Owner: Rachel
Audience: Internal production staff
Cadence: Occasional (as features and editorial mature)

The Production Guide is a practical explanation of formatting and style conventions that should be consistent across Guides. It includes a production checklist to ensure that each of these conventions is met before release of a Guide.

# **Emoji Tagging**

Use emoji from the Emoji Lexicon to alert readers to particular types of information. Emoji help us make our work accessible, by alerting readers to often overlooked information, warnings, controversies, and more. 

## Lexicon

Emoji tags come in media types, friction or quality indicators, importance and social context, technical topics, programming languages, and general content descriptors.

See the full emoji lexicon, regularly updated, [on GitHub](https://github.com/feynmanlabs/lexikon-site/blob/master/pipeline/docs/doc_config_defaults.yml).  

## **Emoji formatting**

* Emojis are used to annotate parts of text and activate features or formatting rules.
* Some emoji should be placed at the** block level**, preceding a paragraph or bullet point. Some should be placed on **link text** only.
* Media type emoji and some quality and friction indicators (when referring to a link) should be in-line next to the URL or linked text. When working in Markdown, these emoji must be placed inside the brackets containing the linked text, as in: “these companies are usually [💰formed in Delaware](https://www.nytimes.com/2012/07/01/business/how-delaware-thrives-as-a-corporate-tax-haven.html).
* The 🚧, which marks additions or elaborations that need to be made or specific questions that need to be answered, precedes the explanatory text at the chunk level, preferably at the bottom of the section where that information will eventually be added. Because it can be confusing to readers, there should be no boldfacing within the text marked by 🚧; when referring to a specific term or definition that needs to be added, italicize the term. 

# **Definitions**

There is an important emoji, 🄳, which we use to mark definitions of essential terms. This section covers production guidelines for definitions.

### **How it works**

🄳 The **defining occurrence** of a term (word or phrase) is the fullest glossary-style definition of that term within a Guide. Often, the defining occurrence is the first time a term is mentioned, but it may be mentioned in passing or incidentally before its defining occurrence. The defining occurrence should include one to three (or so) sentences that define the term for the lay reader.

* The defining occurrence generally looks like the paragraph above. It may first appear in a key terms/concepts/entities section, or in a chapter. 
* When the 🄳 is added at the start of a chunk of text that contains a bolded term, the annotation will make the chunk (a paragraph or bulleted item) the defining occurrence of that term—the official definition of that term that can appear elsewhere in the product, as a searchable definition, as part of a glossary, and in a mouseover.

🄳 A **mouseover** refers to the definition of a term appearing as you hold your cursor over the term (desktop) or quick tap the term (mobile) as it occurs throughout the text.

* Mouseovers also allow you to visit the defining occurrence by clicking (or tapping) on the mouseover text itself. This is important because a reader is able to get the context of the defining occurrence if they need it. Users will be able to jump to the defining occurrence (and see its surrounding text) and then jump back to where they were (this may be a forward and back button in the browser, though the tooling may change down the road). Otherwise, a reader can simply remind themselves of the definition using the mouseover feature and move on with where they were in the text. 
* Mouseovers are helpful because sometimes structure dictates that a term be mentioned before being officially defined; other times, a term may not be mentioned again until a dozen pages after it was defined. A **forward mouseover** occurs over a term that precedes that term's defining occurrence. A **reverse mouseover** refers to a defining occurrence from earlier in the text. 
* Mouseover matches will be for the longest matching phrase. For example, “ownership interest” would have a mouseover definition but “ownership” would not. 
* Some terms are formally defined but are so common (“company,” “property”) they will be configured to have mouseovers disabled globally. 
    * We may in the future develop a way to disable mouseovers on a case by case basis (by adding the ➰ emoji before a specific occurrence). We may also develop a way to override a globally disabled mouseover so that it does appear in certain instances. 

### **Formatting**

* Place the 🄳 at the start of a chunk of defining occurrence text, and follow it with a space.
* It is very helpful to have the 🄳 readily available to you! Bring up the emoji keyboard by pressing (control + command + space bar). Expand the keyboard by clicking the small box in the top right corner. Copy and paste the 🄳 into the emoji search bar, then drag it into the “frequently used” section of your emoji keyboard. Now you can find it easily. 
* Every defined term can have one or more **alternatives**. These might include an acronym or initialism of the term being defined, a shortened version, synonyms, or simply an alternate but relevant phrasing. These alternate terms usually directly follow the defined term in the defining occurrence chunk. They will be supported with mouseover definitions of the defined term if they appear in parentheses, in bold along with the parentheses. In general, use (and bold) “or” within the parentheses if showing an alternate phrase, synonym, or abbreviation; no “or” is needed if showing an acronym or initialism.
    * E.g. “🄳 A **capitalization table (or cap table)** is a [table](https://www.investopedia.com/terms/c/capitalization-table.asp) (often a spreadsheet or other official record) that...”
    * E.g. “🄳  **Annual Percentage Rate (APR)** is the total cost per year of borrowing money, including the interest rate, as well as any [mortgage points,](https://en.wikipedia.org/wiki/Discount_points) fees, charges to create the loan itself...”
    * It may be the case that the best phrasing of a definition separates the defined term and its alternate: 
        * E.g. “🄳 A private company becomes a public company (or '**goes public'**) in a process called an [**initial public offering (IPO)**](https://en.wikipedia.org/wiki/Initial_public_offering)...”
        * Using this example, you will be able to mouseover every occurrence of the phrase “goes public” in the Guide, and the definition of IPO will appear. In the earlier examples, “cap table” and “APR” would bring up mouseovers in the same way.
* Often, only one term will be defined per chunk. But sometimes it makes the most sense to define two terms at once, in contrast or relation to each other. A 🄳 before a chunk that is defining two terms works the same way as with one term. The chunk as a whole, with both terms defined, will come up as a mouseover for either term throughout the text. We call these **joint definitions**. 
    * E.g. “🄳 [**Stock**](https://en.wikipedia.org/wiki/Stock) is a legal invention that represents ownership in a company. [**Shares**](https://en.wikipedia.org/wiki/Share_(finance) are portions of stock that allow a company to grant ownership to a variety of people or other companies in flexible ways.”
    * If a reader invariably will need to understand both concepts at once (in *both* directions, meaning both definitions depend on each other), it's best to have a joint definition. In this example, understanding the terms “shares” or “stock” is impossible without knowing about both.
* We do not prefer to have any other emoji present before a defining occurrence. If there is a quality about a particular definition that needs to be pointed out—a pitfall or confusion, say—make an emoji-tagged statement about that quality in a subsequent bullet. 
* **Boldface usage**:
    * The defined term must be boldfaced. When possible, the boldfaced term should occur **near the front** of the definition, as well as the **defining text** (or the clearest single sentence that precisely defines the fundamental aspects of the term). This makes mouseovers easier to digest, and emphasizes what term  or terms are being defined.
    * Any alternates must be boldfaced, along with the parentheses that hold them. If “or” is part of the parenthetical, it too should be boldfaced.
    * In the case of joint definitions, both defined terms must be boldfaced. 
    * Boldface full terms if the partial term would have misleading mouseovers.
        * E.g. “**long-term capital gains**,” not “**long-term **capital gains”

### **Rules for writing definitions**

Definitions should be the best brief definition available within the context of the Guide, and should include: 

1. A brief, precise definition, close to what an encyclopedia or dictionary might give.
2. Abbreviations or synonyms.
3. Elaboration given context of the Guide (this is essential—what does the term mean specifically in the context of the topic under study? 
    1. E.g. “broker” has a different meaning in the context of buying a home than it does in personal finance.
4. Possible confusions or differentiations, including warnings not to confuse this term with others like it or the same term in different contexts.
5. Any definitive links, including authoritative sources that explore the term or its intricacies further, that correspond to this definition.

* Usually, start with** defining text **(the actual sentences that precisely define the term). Then follow with **explanatory text** (more informal text that tells you what it means or gives additional situational detail).
* Because definitions will appear in a glossary, they are generally more formal than the text that surrounds them. They should be able to stand alone. 
    * Avoid the second person in defining text. Explanatory text that follows defining text can be more informal and employ the second person (particularly when a definition depends upon or leads to some kind of action). 
    * Avoid first person plural in defining text, as in, “We call this X.” 
    * If there is explanatory text in the same paragraph as the main definition, but it is situational or otherwise not important enough to always appear inside a definition, move it to a subsequent  bullet or paragraph. Remember, emoji tagging can be used on bulleted explanatory text that follows the formal definition of a term.
* Avoid uncertain and imprecise language within defining text. Words like “maybe,” “often,” and “typically” can confuse the reader about whether these are defining characteristics or just commentary. The definition itself should be certain, even if its implications are uncertain. These can always be elaborated on later or even after a clear initial explanation. 
    * For example, avoid phrasing like this: “🄳 **Mortgage Insurance (MI)** is a type of insurance that may protect the lender in case you fail to make payments.” 
    * Prefer this: “🄳 **Mortgage Insurance (MI)** is a type of insurance that protects the lender in case the borrower fails to make payments. It typically...” 
* **Referencing other terms**: Do make use of other terms or concepts, and rely on mouseover definitions of other terms within a definition. (A definition will never mouseover the same term already being defined, even if the text appears more than once.)
* An** incidental definition** is when a new term is introduced but for one reason or another, we're not going to define it formally with a full definition. Use *italics* for incidental definitions, **not boldface**. That way, a reader should not have to wonder, “Is this really a definition?” Incidental definitions should not appear within the defining occurrence of another term. 
* **Logical precision**:
    * Be careful about directions of implications so the full sense of the word is clear.
    * For example, the defining statement “X is a situation where Y” is not the same as “In situation X, Y happens” or “Y occurs when X.” The first is a precise definition since it means "X implies Y *and* Y implies X," while the latter two both mean *only* "X implies Y." 
    * Yes:
        * “An **acquisition** is when one company purchases more than 50 percent of another company.”
        * **“Dilution** is when percentage ownership of each shareholder goes down as the number of outstanding shares goes up.”
        * “As the number of outstanding shares goes up, the percentage ownership of each shareholder goes down. This is called **dilution**.”
    * No:
        * “In an **acquisition**, one company purchases more than 50 percent of another company.” (Do other things need to happen as well for this to be an acquisition?)
        * **“Dilution** occurs as the number of outstanding shares goes up and the percentage ownership of each shareholder goes down.” (Are other things occurring too? Does dilution itself mean more than this?) 
* **Links**: Do make helpful links to external resources and internal sections if appropriate
    * **Section links**: Forward (and reverse) mouseovers very often make internal section links unnecessary for specific concepts. But sometimes definition links should be replaced by forward (and reverse) section links if appropriate, such as if it's the subject of an entire section.
    * Prefer to keep external links attached to alternative terms or wherever they are most appropriate in the definition, avoiding (though this is not always possible) linking the defined term itself.
        * E.g. Wikipedia or Investopedia definitions for further elaboration, or the main websites of a person or entity closely associated with the defined term.

### **Rules for sequencing definitions**

* **Don't define things twice**: The defining occurrence should only be in one place. If the reader is already expected to understand a term, avoid re-stating a definition again in similar form a second place. The mouseover will be sufficient.
* A Guide should be understandable if read front to back, even without mouseovers.
    * That is, even though mouseovers will add a lot of convenience, we're not abandoning the editorial responsibility of organizing the definitions.
    * Structurally this is *still* like a book in key ways. Thinking about sequencing helps us organize material, have editorial discussions on organization much like a book, and source authors much like a book too—but with the convenience that a lot of language (like “see the section on X”) can be omitted.
    * Forward mouseovers should be used for convenience *but not to dispel confusion.*
* **Where to put definitions**: Defining occurrences should be wherever they best fit common usage by the reader:
    * To consider where a definition goes, ask: If a reader doesn't understand X, what *other* things should they be reading about?
    * Foundational definitions that are likely to be mentioned should go earlier, often in foundational sections (names TBD and may vary by topic).
    * Advanced things should go in advanced sections, likely grouped with other advanced definitions on that topic, or for that phase of the process, etc.


🚧 We may bring in “Requirements” and “Our Approach” from [Definitions and Glossary Guidance](https://quip.com/DW8IA4tUZcqe).

# **Linking & Citations Formatting**

## Guidelines for linking

For each sentence we write, we ask ourselves, what is the best link giving detail on this or verifying it?

* For each link added, we ask, is this really a good link, or is there a better one? Is the link to a summary when a primary source would be better? Is the linked source actually selling something, meaning we need to dig deeper?

In general, links are needed when:

* Referencing anything but a personal story, folkloric wisdom, or common knowledge.
* Any statement where a curious reader might ask, “How do they know that?”
* The information provides a reference to any number.
* Imagining relative amounts, like “most people,” “hardly anyone,” or “rarely.”
* Referencing a study, book, article, figure, or person.
* When verifying or mitigating an assertion or popular opinion.
* When elaboration or detail on a concept, idea, or example can reasonably be considered outside the scope of a Guide. Prodigious linking to great resources that cover material not necessarily within the scope of the Guide can also be found in Further Reading sections (see below).
* 🔸 If a contributor includes information that comes from their experience or expertise, readers still need verification from other sources.

### Linking to people, places, things, companies, and events

* For well-known people, places, things, and events, we link to the Wikipedia page.
    * If there is a good quality Wikipedia page, prefer it to company or organization home pages, home pages of cities, states, or agencies, or personal or promotional websites.
    * Why? Wikipedia editors are not trying to sell anything. Wikipedia entries usually gives more context to the reader than a company page, and by linking to a free and trusted source we save readers having to Google to find more.
        * It will also help with our search and web page snippet features, since the mouseovers on the links will be better quality than for those on marketing pages or poorly organized or out-of-date official websites.
        * This might look like: “The [Bay Area](https://en.wikipedia.org/wiki/San_Francisco_Bay_Area) in [California](https://en.wikipedia.org/wiki/California) is home to both [Apple](https://en.wikipedia.org/wiki/Apple_Inc.) and [Google](https://en.wikipedia.org/wiki/Google).”
    * Of course, there’s not a Wikipedia article for everything. Or sometimes the article is of inferior quality to another resource on the web. In those cases, we do our research and link to the best page we can find.
* For tools or anything practical, we provide a link to the original resource to readers, not a write-up of it by a third party. Where the resource has costs associated with it, we’ll alert readers using emoji tagging.
* Some organizations, say the California DMV or Yosemite National Park, might require both a Wikipedia link for context on that organization and a homepage link for tools or resources. If, given the context of the Guide, a single link is clearly most useful, that’s what we’ll provide.
* We’ll also link to the Wikipedia page of most individuals mentioned. However, many contemporary figures' primary online presence is their website, their Twitter profile, or their LinkedIn or Medium profile. Given context, one or more of those may be most appropriate to provide to readers.

## Link formatting

Inline links are links that appear within sentences, attached to appropriate words or phrases in the sentence called “linked text” or “anchor text.” This is in opposition to, say, a list of links we might provide in a section like Further Reading. There are two types of inline links, internal and external. Some formatting is the same for both:

* Prefer the most descriptive and logical set of words as anchor text that give a clue to the linked page or linked internal section.
* Given that, prefer shorter anchor text. Long, highlighted links (with mouseovers), especially more than five words or so, tend to be distracting and ugly.
* Best practices for anchor text are also [guided by how SEO works](https://moz.com/learn/seo/anchor-text).
* Do not include parentheses or quotation marks in the linked text.
* If linking a term or phrase that must be boldfaced, the Markdown code for boldfacing should appear inside the brackets that contain the linked text.
    * E.g. [****This phrase****](link)
* Multiple links should not appear directly next to each other. Except in the case of a list of items where an unlinked comma separates two sets of linked text, spread out multiple links so that they do not appear as one to the reader.
* Do not include articles like “a” or “the” in the linked text.

### External links

* Say *less* with a link, not more. Rather than citing a source from which the definition of the term stated was derived, this link acts as its own citation, moving a reader to the in-depth resource:
    * “The Security and Exchange Commission (SEC) regulates accredited investors, a term which refers to individuals who meet [certain net worth or income standards](http://www.investopedia.com/terms/a/accreditedinvestor.asp). Before accepting money…”
* Prefer actionable words or phrases in a sentence if the action or assertion is the primary point. Prefer the verb or verb phrase over the object alone:
    * “Even if you’re busy, you can [get started easily](https://www.psychologytoday.com/blog/in-practice/201303/5-meditation-tips-beginners).”
* Nouns can work too, optionally including the adjectives or other parts of the phrase, depending on length and clarity:
    * Best: “According to a[2014 New York Times article](https://www.nytimes.com/2014/05/22/upshot/rent-or-buy-the-math-is-changing.html), …”
    * Still good: “According to a 2014 New York Times [article](https://www.nytimes.com/2014/05/22/upshot/rent-or-buy-the-math-is-changing.html), …”
        * The second choice may be preferred if nearby text has additional links, and linking a longer phrase would look clunky.
* In particular, avoid linking in a way that leads the reader to think you’re linking a specific noun:
    * Not: “*Venture* is defined by [Merriam-Webster](https://www.merriam-webster.com/dictionary/venture) as …”
    * Not: “According to a 2014 [New York Times](https://www.nytimes.com/2014/05/22/upshot/rent-or-buy-the-math-is-changing.html) article …”
* ❗️ Avoid using completely generic, self-descriptive anchor text that tells the reader to “read this” or “click here.”
    * Acceptable but not ideal: “For more details, [read the full article](https://www.nytimes.com/2014/05/22/upshot/rent-or-buy-the-math-is-changing.html).”
    * Not: “An article about this is [here](https://www.nytimes.com/2014/05/22/upshot/rent-or-buy-the-math-is-changing.html).”
    * Please, never: “[Click here](https://www.nytimes.com/2014/05/22/upshot/rent-or-buy-the-math-is-changing.html) to read more about…”

### Internal links

Cross referencing (linking to material that appears in another place within the Guide) is important to the internal discoverability of our content. We call these internal links or “anchor links” (not to be confused with "anchor text"), and they help direct readers to further information on a component of a topic that might be mentioned elsewhere in a Guide. 

Linking to internal text is different from linking to external text. If there is a section called “Hello There!” we link to it [like this](#hello-there). Make sure to follow each of these directions: 

* Lowercase the text.
* Remove everything that is not a letter, number, space, or hyphen ([see here](https://gist.github.com/asabaylus/3071099) for how Unicode is handled).
* Change spaces to hyphens.
* If a section title is not unique (this is very rare!), add “-1”, “-2”, “-3”, etc. to the link to make it unique.

Other considerations:

* Rather than link a secondary occurrence of a term to its defining occurrence using an internal link, remember that the mouseover feature will render most links to internal definitions unnecessary.
* An internal link should be used when more context is needed or in the case that a reader may want to jump to another section for the answer to a specific question. Prefer forward links when:
    * Gesturing to topics covered next, like a roadmap.
    * Mentioning things that are technically related but were not appropriate to cover. For example, a parenthetical note mentioning how something relates to a topic covered in depth later.

### Further reading

We keep track of resources that will be helpful to readers interested in furthering their knowledge of a Guide’s subject. Resources can include online works that are foundational, are notable general resources, or are deeper explorations of important sub-topics or components of the larger topic of a Guide. We also note longer format works that are out of the scope of the Guide, including books and movies. Additional resources, like tools and documents, may also be provided. The Further Reading section is the last section of a Guide before its disclaimer and credits. It is essentially a bibliography of suggested resources, arranged by topic, and tagged with emoji. 

* The heading “Further Reading” is an H2 heading (see Headings, below).
* For each citation, list the author, publisher or organization responsible for the content (if applicable), the linked title of the piece, and the year of publication. The format is:

    * First Last, Organization,* Title,* Year.
    * E.g. “Andy Rachleff, Wealthfront, [*How Do Stock Options and RSUs Differ?*](https://blog.wealthfront.com/stock-options-versus-rsu/), 2014.”
    * We favor this simplified citation format because it can accommodate most of the resource types you're likely to encounter such as blogs, magazine and newspaper articles, and academic works.
* Citations should be tagged with the appropriate emoji if they are paywalled or require login.  They should also be tagged if they are documents (like links to resume forms in a Guide to Choosing a Career) or tools (like a mortgage calculator in the Guide to Buying a Home).
    * Example: Orrick, [📥 Startup Forms: Equity Compensation](https://www.orrick.com/Total-Access/Tool-Kit/Start-Up-Forms/Equity-Compensation)
* Citations should be grouped into topics, which are bolded (they are not headings) and followed by the bulleted list of citations. 
    * There should be a variety of topics including general resources, resources geared toward specific groups of readers,  sub-topics relevant to the Guide, and documents and tools. 
    * Most Guides will contain the Further Reading topics “General resources” and “Documents and tools” but other topics are Guide-dependent. 
        * E.g. In the Guide to Equity Compensation, topics include “Considerations for founders” and “Considerations for candidates and employees” (for links of particular interest to certain readers) and “Taxes” and “Negotiation” (as important sub-topics). 
* Each topic should be ordered according to relevance to the Guide and interest to the general reader. Core topics should occur at the top, with more specific subjects occurring further down.
    * The ordered list of topics in the Guide to Equity Compensation: **General resources, Considerations for founders, Considerations for candidates and employees, Types of equity compensation, Taxes, Vesting and expiration of stock options, Negotiation, **and** Forms and tools**.
* Citations under a topic should be bulleted and ordered by the author's last name. Citations without specified authors should occur at the end of the topic's citation list, ordered alphabetically by title.
* Please refer to the [Further Reading section](https://www.holloway.com/g/equity-compensation#further-reading) of Equity Compensation for visual guidance.

# **Style Guide**

This is a growing  list of copyediting and proofing conventions favored by Holloway, each of which must be checked by the editorial team before release of a Guide. 

## Punctuation and grammar

### Punctuation 

For instructions on use of the comma; colon; semicolon; hyphen; em dash; en dash; parentheticals; brackets; and full stops or periods, refer to the Chicago Manual of Style's guidance [on punctuation](https://www.chicagomanualofstyle.org/16/ch06/ch06_toc.html) or check with a senior editor.

There are a few helpful reminders of punctuation that tends to come up a lot in Holloway Guides, and which should be checked thoroughly for consistency within and across Guides before release of any Guide or portion of a Guide: 

1. **Colons**: Use when introducing a list of bullet points or steps (more on lists below). 
2. **En dashes**: Use to combine numerals (in “10-20,” the en dash means “through” or “to”), or to combine subjects that have equal weight, as in, “The British-American economist...” (more on numbers below).
    1. If you use a Mac, the en dash can be typed as ⌥-.
3. **Em dashes: **These must must not have spaces around them. 
    1. If you use a Mac, the em dash can be typed as ⇧⌥-. 
4. If working in GitHub, running **Flowmark** will correct em dashes formed with two hyphens, convert hyphens to en dashes between numerals, and orient quotation marks and apostrophes in most cases.
    1. Trailing apostrophes (as in “Sanders'”) need to manually oriented.
    2. Non-oriented quotes appearing next to other punctuation may need manual attention as well.
5. **Quotation marks** offset titles of blog posts, essays, and articles. 
6. **Punctuation marks** should match the font and formatting on the sentence they belong to. Exception are:
    1. Do not boldface the colon in inline headings. 
    2. Formatting of punctuation contained in a quote should match the formatting of the original quote. 
7. **Oxford comma**: Holloway prefers consistent usage of the Oxford or serial comma. 

### Grammar and usage

For any grammar and usage confusion, refer to the [Chicago Manual of Style](https://www.chicagomanualofstyle.org/book/ed17/part2/ch05/toc.html). 

Listed here are Holloway's preferences when it comes to some usage issues, all of which should be checked thoroughly for consistency within and across Guides before release of any Guide or portion of a Guide:

1. **Okay**, rather than OK or ok. 
2. **Toward(s)**: Adding the 's' to “toward” and “forward,” etc., is normal in Britain; in America the 's' is elided. 
3. **E.g.** means “exempli gratia,” or “for example.” **I.e.** means “id est,” or, “that is.”
    1. In general text we prefer “for example,” “like,” and “that is” or “as in” over the Latin, excepting in examples of data. 
4. **Internet**: Unless it's starting a sentence, we prefer not to capitalize internet. 
5. **Adverbs**: “The road to hell is paved with adverbs,” quoth Stephen King. Avoid them. 
6. **Gender neutral pronouns**: When referencing a real person, be certain that you are using that person's preferred gender pronoun. You can often find this information on a person's Twitter, personal homepage, or Wikipedia page.
    1. When referring to a person who does not identify with the gender binary, and no personal preference is known or available, Holloway prefers "they," "them," and "their" pronouns.
    2. In a series of examples, make sure that not every example uses "he," "him," "his." It is best to alternate between "he," "she," and "they” where clear.

## **Formatting**

**Italics**
Italics should be used when referencing book titles; the names of blogs; newspapers, magazines, and periodicals. We also use italics specific to Holloway in the following ways: 

* When referring to an example of a word rather than a word in context. 
    * People often put examples of words in quotation marks, but this can be confusing if a text already includes quoted material, and it also tends to look quite bulky.
* Prefer italics over boldface for incidental definitions, and italicize terms that we hope to define later when laid out under a 🚧 emoji.

### 🚧 Boldface

Use boldface when you really want to offset something important or surprising. It can actually be helpful to do this as you write, because it can alert us to product features and graphic design opportunities we might employ.

* Boldface defining occurrences of terms (see Definitions) 
* Key statements: It’s also fine to boldface key statements and phrases that guide the eye.
* As has been said, we try to avoid boldface for incidental definitions, preferring italics. Prefer italics for terms of future definitions marked off with 🚧.

🚧 Rules for boldfacing defining occurrences and numbers are clear; we lack clear direction for boldfacing key or surprising phrases. In Equity Comp, for example, there is plenty of boldfacing of key phrases in the introductory content, but we rarely use this convention elsewhere in the Guide.

🚧 Our current style rule dictates bolding of key phrases, but we might consider amending this for more frictionless reading--Because of the importance of bolding defining occurrences, it may be confusing to readers when we do not implement the tactic consistently (we have received this feedback). (I have noted where we've bolded inconsistently in EC in Production Editorial Checklist (Quip).

### **referencing Quantitative data** 

* Numbers one through ten should be written out.
* 11 and up should be numerals.
* An en dash—not a hyphen—is used to show a range of numbers, as in “9–20.”
    * If you’re only using numbers below 10, write it out, as in “one through three” or “one to three.”

Key statistics often pop up and are much more readable in **boldface**. 

* Numbers that are key statistics or worth paying attention to should be in boldface.
    * "The population of Botswana is **2.3 million** and its GDP is **$41.6 billion** US dollars."
* Include the percentage symbol or units in bold.
    * **$5M dollars** or **10%** or **153,000**
* Do not boldface illustrative or example numbers, or numbers that are written out as words.
    * "For example, if you have 24 apples equally divided in two buckets..."
* When using a single letter as shorthand for a quantity, e.g. M for million or K for thousand, the letter should always be capitalized and there should be no space between the letter and the number. 

### Figures and tables

Thanks to the UNC Writing Center for help with this section.
If you can summarize the data in a figure or table in one to two sentences, do so. If your data are more numerous, providing a figure or table for representation can be helpful and keep text from getting cluttered with numbers.

* Keep track of any ideas you have about how data can be used in a Guide and share with our engineers and design team.
* A *table* is a columned list of raw data, numbers of text, and is not designed to show the relationship between any variable. Tables should be:
    * Numbered
    * Centered on the page and set apart from the text.
    * Titled, where the title appears on top of the table (Do not rename it if it already has a name.)
* *Figures* are maps, graphs, charts, drawings, or photos. These are what you use when you’re trying to share a conclusion about your data in the form of relationships between variables. Figures should be:
    * Numbered (e.g. “Figure 1”)
    * Centered on the page and set apart from the text.
    * Captioned, with the caption appearing below the figure.

### Lists

Lists are extremely important to the flow and readability of Guides. We use two types of lists, bullet and numbered.

* Use numbered lists only when laying out steps that should be taken *in order*.
* Use bullet lists for everything else. If the paragraph before the list ends in a colon and the list is an itemization:
    * start each point with a lowercase letter
    * don’t punctuate the end of the line
    * but finish the last piece in the list with a full stop.
* If there is no preceding semicolon, the bullets should each represent a different, separable piece of relevant information that can stand apart from others in the list and still be understood. It may happen that a colon precedes a list of items that are separable and stand-alone. 
    * If your bullet points stand alone, use a capital letter to start each one, and a full stop to end each one.

### Headings

**Main headings**: Headings come at different levels: title, section or chapter, sub-section, and so on. We refer to these as H1, H2, and H3. These correspond to HTML levels (that is, the actual codes used on websites) as well as Markdown levels (one, two, or more # signs).

* H1 = # =  main title
* H2 = ## = main sections
* H3 = ### = sub-sections
* Capitalize each word (excluding articles and conjunctions) in section titles at H1 and H2 level, and *do not* capitalize after the first word in section headings for H3. Deeper than H3, prefer inline headings.
* For headings and titles, we prefer to spell out “and” rather than use an ampersand. 

**Inline headings**: These are headings like this one, which are at the head of a paragraph (not H2 or H3). We often use them to guide the eye where a main heading is excessive, or to label each paragraph in a bulleted list of items.

* **Boldface** inline headings. Avoid inline headings that are plain roman.
* Do not boldface the colon, but do maintain other formatting (like italics) with all other punctuation (like exclamation points or quotation marks).
* Prefer to use inline headings on paragraphs or most (or all) items in a bulleted list, but not only one or two items in a bulleted list.


🚧 More guidance needed on section headings; inline heading formatting; lists; and boldface preferences (under discussion).

# **Production Checklist**

This is a summary of the details discussed in this Production Guide. Each of these should be checked off by at least two people before releasing a Guide. 

## Copy edits

* **Language for clarity and style**
* Punctuation
    * All oriented quotes and apostrophes
        * Check common cases: Search for s' and non-oriented quotes and fix all
    * Em dashes and en dashes
* Consistent use of capitalization and hyphenation
    * Especially on terms with ambiguous capitalization (e.g. Alternative Minimum Tax) or hyphenation (e.g. startup/start-up) 
    * Double check capitalization w/in inline headings. 
* Formatting
    * Language formatting
        * Section headings according to style (capitalizations, etc.)
        * Consistent use of boldface
        * Consistent use of italics vs quotes
* Structural formatting
    * Bullet usage at chunk level
        * We sometimes use paragraphs and sometimes bullets. Validate there is a reasonable balance, using bullets judiciously.
            * Key pieces of content that fit together in a narrative way are good as paragraphs.
            * Bullets and sub-bullets encouraged whenever there is a laundry list of items, or three or more items fit together in a natural way, or the list may expand in the future via contributions. But not over-done or many levels deep.
    * Roadmap is clearly organized and all forward links are correct and make sense.
    * Boldfacing of enumerated item headings
        * If every item of a bulleted list has a small inline heading (with a colon), boldface all of them.
            * Exception: No need to bold lists of subjects under examination, eg. “Hire 1:; Hire 2:”, even if each example is followed by a colon, and especially if the explanatory text contains bolded text like numbers. 
    * Emoji usage according to style
        * For block level emoji, each chunk is styled as expected.
        * Watch out for wrongly-tagged blocks. (E.g. is it a confusion or a warning?)
* Definitions
    * Definitions terms
        * Use of joint definitions and abbreviations or alternates appropriately.
    * Definitions semantics and clarity
        * Logic of definitions
        * Sequencing makes sense
    * Use of links within definitions
        * Prefer external definitive links on the defining occurrence itself or on verbs or somewhere else suitable
        * FUTURE: Consider a way for us never to link of the defining occurrence (may require a product change). We'll avoid using the term being defined in a defining occurrence as linked text. For now, this is fine where it does not add confusion, though we prefer verbs or other suitable phrases within the defining occurrence to be the linked text to an external definition. 
    * Placement
        * No definitions within a bullet list unless really clearer that way
        * When there are a lot of definitions, group them adjacently in a way that aids clarity
    * Incidental definitions
        * Terms not properly worth being joint definitions should be incidental (so italics)
        * Italics within definitions only used for emphasis, not for introducing new terms
    * Definitions occurrences
        * Mouseovers appearing where helpful, neither inappropriately or missing when expected
        * Double check all substitutions (abbreviations, initialisms) as well as terms that might have a noun present in a defining occurence suspended as when relating two terms: E.g. “public and private company”; “preferred and common stock”. In those instances, only “private company” and “common stock” would get mouseovers— confusing! Change to “preferred stock and common stock,” for example.
    * Review blacklist decisions and verify they're appropriate
        * FUTURE: Use a report on usages and occurrences 
        * FUTURE: A few case-by-case fixes once we have support
* Links
    * Internal links valid (will use Atom plugin or pipeline report)
    * Internal links where appropriate
        * Not used when definitions mouseovers would do
    * External links
        * Check mouseovers (for quality and to ensure links are valid—a broken link (404) will only show the domain name in mouseover (but so will .pdfs) so click all such links).
        * For each, ask: Is anchor text, placement in sentence or paragraph, and link itself right?
        * Is snippet acceptable? (Some imperfections are tolerable but anything misleading or bizarre should be addressed.)
    * Make sure no two sets of linked text are directly next to each other. There should be at minimum one word between two sets of linked text. 
    * Emoji link tagging
        * Paid and login links marked
        * Media type emojis
            * Paid
            * Loginwall
            * Download
            * Tool
* Research
    * For topics that might have changed recently (like tax rates), links are current
* Further Reading
    * Fits consistent style, grouped clearly with boldface (not section) headings
    * Each entry a top-level bullet (chunk) so it shows up individually in search
* Data (we offer a lot of inline percentages, we could start there)
    * Data is fact-checked and accurate
    * Data is cited
* Graphics
    * Working on desktop and mobile
* Tables
    * Working on desktop and mobile
* Document settings
    * Masthead is correct, current, and complete
    * Twitter, web, and/or GitHub links for each contributor are confirmed
    * Number of contributors is set
    * Tagline at top of Guide
    * Legend is clear
* Marketing and social media
    * Messaging
    * Images for sharing
    * Testimonials

 

