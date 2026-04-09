# Create-LinkedIn-Company-Post
This workflow automates the process of publishing posts to a LinkedIn company page by handling everything from input validation to final posting. It starts with a webhook that receives a request containing the post type (text, article, image, or video) along with required content. The workflow validates the input and routes it through different branches based on the post type to ensure the correct format is used.

For each post type, the workflow prepares and sends the appropriate request to LinkedIn’s API, including fetching access tokens and company details. In the case of media posts like images and videos, it also handles uploading files by registering the asset, downloading the media, and then uploading it to LinkedIn before creating the post.

Additionally, the workflow includes strong error handling and validation steps to ensure all required fields are provided. If something is missing or incorrect, it returns clear error messages. Once successful, it responds with confirmation and post details, making the entire publishing process fully automated and reliable.
