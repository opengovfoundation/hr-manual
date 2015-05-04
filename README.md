# hr-manual
## Human Resources Manual for reuse

This is a series of documents we're using at the The OpenGov Foundation, created by ourselves with our laywers. Creating a strong human resources policy is an expensive, difficult task for most small organizations.

All of these documents are being released with open licenses, meaning they're **absolutely free to use**.  This will allow any person or organization - **for profit or not for profit** - to copy, edit, rewrite, and distribute them at no cost!  The majority of them are [Creative Commons CC0 Licensed](https://creativecommons.org/publicdomain/zero/1.0/), dedicating them to the public domain.

There are a variety of documents here which may or may not be relevant to your organization, so feel free to use whichever of these are useful and ignore the rest.

Included are:

* [HR Policy Manual](./markdown/manual.md) - The policy manual we're using at OpenGov Foundation, covering benefits, company policies, and more.
* [Holidays](./markdown/holidays.md) - A full list of the days the organization is officially closed.

Please suggest any changes that you think we should make, or contribute your own to the repo!

There are other useful documents to use in our [HR Resources Repository](https://github.com/opengovfoundation/hr-resources).


## Disclaimer
This was created based on United States law, and if you're not in the US the policies here might not be legal wherever you are.

We are not lawyers, and cannot give you legal advice or tell you what is best for your organization. If you have any questions, ask an actual lawyer.

## Available Files

The following files are available in a variety of formats - use the links below to download them directly.

Document | Description | | | |
--- | --- | --- | --- | --- |
HR Policy Manual | [Markdown](https://rawgit.com/opengovfoundation/hr-manual/master/markdown/manual.md) | [HTML](https://rawgit.com/opengovfoundation/hr-manual/master/html/manual.html) | [PDF](https://rawgit.com/opengovfoundation/hr-manual/master/pdf/manual.pdf) | [Microsoft Word](https://rawgit.com/opengovfoundation/hr-manual/master/docx/manual.docx)
Holidays (2015-2016) | [Markdown](https://rawgit.com/opengovfoundation/hr-manual/master/markdown/holidays.md) | [HTML](https://rawgit.com/opengovfoundation/hr-manual/master/html/holidays.html) | [PDF](https://rawgit.com/opengovfoundation/hr-manual/master/pdf/holidays.pdf) | [Microsoft Word](https://rawgit.com/opengovfoundation/hr-manual/master/docx/holidays.docx)

## Contributing

We welcome suggested edits to these documents!

We use Markdown as the primary format for these files, so you'll need to know a little before you begin. Don't worry - it's easy!  [Here's a quick guide.](https://guides.github.com/features/mastering-markdown/) If you've used a wiki, reddit, etc. it should be easy to pick up.  *Note that we _cannot_ accept changes directly made to other formats, only Markdown.*

If you don't want to learn Markdown and still want to contribute, feel free to [open an issue on this repo](./issues), or just [send us an email](mailto:sayhello@opengovfoundation.org).

### The Easy Way ###
You can edit the files directly using the links below, no account or GitHub experience needed!

*Coming Soon!*

### The Advanced Way ###
If you are familiar with GitHub, please fork the repo and send a pull request.

We use [pandoc](http://pandoc.org/) to generate the many formats we display.  If you don't have pandoc installed, that's ok!  Just send us a pull request with the updated markdown files.

If you have pandoc installed with pdfLaTeX, you can run the following command from the repository root to generate these files:

    for myfile in $( ls ./markdown ); do echo Converting $myfile; for fmt in html docx pdf; do filetrim=${myfile%???}; pandoc -o "./"$fmt"/"$filetrim"."$fmt -f markdown "./markdown/"$myfile; done ; done


