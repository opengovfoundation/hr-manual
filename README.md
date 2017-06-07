# hr-manual
## Human Resources Manual for reuse

This is a series of documents we're using at the The OpenGov Foundation, created by ourselves with our laywers. Creating a strong human resources policy is an expensive, difficult task for most small organizations, so feel free to build off our work to streamline the process for your organization.

All of these documents are being released with open licenses, meaning they're **absolutely free to use**.  This will allow any person or organization - **for profit or not for profit** - to copy, edit, rewrite, and distribute them at no cost!  They are [Creative Commons CC0 Licensed](https://creativecommons.org/publicdomain/zero/1.0/), dedicating them to the public domain.

There are a variety of documents here which may or may not be relevant to your organization, so feel free to use whichever of these are useful and ignore the rest.

For now, we've included the following:

* [HR Policy Manual](./markdown/manual.md) - The policy manual we're using at OpenGov Foundation, covering benefits, company policies, and more.

Please suggest any changes that you think we should make, or contribute your own to the repo!

There are other useful documents to use in our [HR Resources Repository](https://github.com/opengovfoundation/hr-resources).

## Disclaimer
This was created based on United States law, and if you're not in the US the policies here might not be legal wherever you are.

We are not lawyers, and cannot give you legal advice or tell you what is best for your organization.  You should have an actual lawyer review these documents before you use them in the first place.  If you have any questions, ask a lawyer.

We cannot be held responsible for any legal trouble that these documents get you into.  You're using them of your own accord.  We're providing them as-is with no warranty.  Seriously, please don't sue us.

## Available Files

The following files are available in a variety of formats - use the links below to download them directly.

Document | Description | | | |
--- | --- | --- | --- | --- |
HR Policy Manual | [Markdown](https://rawgit.com/opengovfoundation/hr-manual/master/markdown/manual.md) | [HTML](https://rawgit.com/opengovfoundation/hr-manual/master/html/manual.html) | [PDF](https://rawgit.com/opengovfoundation/hr-manual/master/pdf/manual.pdf) | [Microsoft Word](https://rawgit.com/opengovfoundation/hr-manual/master/docx/manual.docx)
Holidays (2015-2016) | [Markdown](https://rawgit.com/opengovfoundation/hr-manual/master/markdown/holidays.md) | [HTML](https://rawgit.com/opengovfoundation/hr-manual/master/html/holidays.html) | [PDF](https://rawgit.com/opengovfoundation/hr-manual/master/pdf/holidays.pdf) | [Microsoft Word](https://rawgit.com/opengovfoundation/hr-manual/master/docx/holidays.docx)

## How to Use The Documents

To use these files, simply download your preferred version and edit them.  You'll probably want to replace the OpenGov-specific information - our staff, board, mission, etc. with your own.  Then read through each section and modify it to fit your own organization's policies and tools.

You'll need to review the final, edited document with a lawyer to make sure everything is legal.  In particular, there are very specific requirements in the US for discrimination, leave, and other workplace practices that you want to get right, or you could face legal action.

To repeat: we are not lawyers!  These documents are meant to be guidelines only to get you started.

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


