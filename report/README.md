# Power BI report asset status

The original source folder contains a loose Power BI report definition (`Report/definition` JSON files), a `DataModel` binary, and supporting metadata. No `.pbix` file or self-contained `.pbip` project entry point was found. These loose artifacts are not copied here because the report/model package cannot be verified as a complete, portable project and the model may contain the customer-level source data.

The four supplied screenshots are included in [`../screenshots/`](../screenshots/). The Customer & Returns preview obscures the customer-level detail table; the original image remains unchanged in the user's source folder. To make the report directly interactive for reviewers, export/share a verified `.pbix` or complete Power BI project after checking its data and sharing rights.
