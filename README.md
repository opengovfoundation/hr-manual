# hr-manual
## Human Resources Policy Manual for reuse

This is the policy manual we're using at The OpenGov Foundation, created by ourselves with our laywers. We are releasing it here under the [CC0 License](https://creativecommons.org/publicdomain/zero/1.0/), so that everyone can take it and reuse it.  Creating a strong human resources policy is an expensive, difficult task for most small organizations.  Feel free to use this for your organization, and please suggest any changes that you think we should make.

## Disclaimer
This was created based on United States law, and if you're not in the US the policies here might not be legal wherever you are.

We are not lawyers, and cannot give you legal advice or tell you what is best for your organization. If you have any questions, ask an actual lawyer.

## Available Files

The following files are available in a variety of formats - use the links below to download them directly.

Document | | | | |
--- | --- | --- | --- | --- |
HR Policy Manual | [Markdown](https://rawgit.com/opengovfoundation/site-policy/master/markdown/manual.md) | [HTML](https://rawgit.com/opengovfoundation/site-policy/master/html/manual.html) | [PDF](https://rawgit.com/opengovfoundation/site-policy/master/pdf/manual.pdf) | [Microsoft Word](https://rawgit.com/opengovfoundation/site-policy/master/docx/manual.docx)
List of Holidays | [Markdown](https://rawgit.com/opengovfoundation/site-policy/master/markdown/holidays.md) | [HTML](https://rawgit.com/opengovfoundation/site-policy/master/html/holidays.html) | [PDF](https://rawgit.com/opengovfoundation/site-policy/master/pdf/holidays.pdf) | [Microsoft Word](https://rawgit.com/opengovfoundation/site-policy/master/docx/holidays.docx)

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


