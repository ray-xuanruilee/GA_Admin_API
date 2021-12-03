# GA_Admin_API
I go through a step by step guide on utilizing Google Analytics' Admin API.

**The guide includes:**
1. Quick look at setting up a Virtual Environment for your Jupyter Lab (Optional)
2. Setting up the Google Analytics Admin API Python Client Library
3. Reference links & resources
4. Using Google Sheets with Python (Optional)
5. Steps on: I. Pulling data from your Google Sheet, II. Creating new GA4 Properties based on data from your Google Sheet, III. Creating new Web Data Streams within the GA4 Properties, IV. Updating your Google Sheet with thew newly created GA4 Properties and Web Data Streams' Measurement IDs, V. Quick guide on deleting GA4 Properties

**Fixes:**
1. I made a mistake in Line 31: 
web_data_stream=WebDataStream(
            default_uri="https://www.google.com", display_name="Test web data stream"
        ),
2. Should be:
web_data_stream=WebDataStream(
            default_uri=ga_web_stream_uri, display_name=ga_web_stream_name
        ),
