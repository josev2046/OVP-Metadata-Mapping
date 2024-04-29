**Context:**
This implementation is designed to facilitate data management, mapping and migration tasks related to video content across two disparate online video platforms (OVPs).

**Story:**
As a user, I aim to retrieve details for a specified list of videos identified by their IDs. This includes gathering essential information such as title, description, tags, thumbnail URL, and download URL for each video. Additionally, I need access to any custom metadata profiles associated with each video.

**UML Sequence Diagram:**

![OVPMetadataMapping](https://github.com/josev2046/OVPMetadataMapping/assets/15835851/8b7d3514-8056-4446-8375-cdac4f2f3f79)




**Breakdown:**
The script leverages an OVP's API to fetch precise details for a set of videos identified by their unique IDs. It gathers vital information like title, description, tags, thumbnail URL, and download URL for each video, while also fetching any custom metadata profiles linked to the videos. By acquiring these attributes, the script facilitates the streamlining of migration tasks across various platforms, exemplified in this case by the transition between Kaltura and Vimeo.

	•	Data Retrieval: The script utilizes the API endpoints to fetch video details and custom metadata from the source OVP.
	•	Error Handling: It incorporates error-handling mechanisms to manage any issues encountered during the data retrieval process.
	•	Data Structuring: The retrieved data is organized and structured into two formats: XML and CSV, tailored to meet the specifications of the target OVP.
	•	XML Output: Video details are neatly organized within <videos> and <video> elements in the XML output.
	•	CSV Output: The CSV output generates a tabular representation with columns for video attributes.
	•	Completion Message: Upon successful completion, the script informs the user of the creation of XML and CSV files, signaling the completion of the data processing task.
