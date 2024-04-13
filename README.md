# Sentiment Analysis API

This API allows you to analyze the sentiment of text input. It uses TextBlob for sentiment analysis.

## Usage

### Endpoint

- **Base URL**: Replace `[base_url]` with the base URL where your API is hosted.

### Analyze Sentiment

#### Request

- **URL**: `[base_url]/sentiment-analysis/{text}`
- **Method**: GET
- **Path Parameters**:
  - `text` (required): The text you want to analyze the sentiment of.

#### Response

- **Body**: JSON object with the following fields:
  - `text`: The input text.
  - `sentiment`: The sentiment of the text (`positive`, `negative`, or `neutral`).
  - `polarity`: The polarity score of the text.
  - `subjectivity`: The subjectivity score of the text.

### Redirect

- **URL**: `[base_url]/`
- **Method**: GET
- **Response**: Redirects to the API documentation.

## Example

### Request

```http
GET [base_url]/sentiment-analysis/This%20is%20a%20great%20day
```

### Response
```
{
    "text": "This is a great day",
    "sentiment": "positive",
    "polarity": 0.8,
    "subjectivity": 0.75
}
```

### How to Run
1. Clone this repository.
2. Install the dependencies by running pip install -r requirements.txt.
3. Run the FastAPI application by executing uvicorn main:app --reload.

### Contributing
Contributions are welcome! Feel free to open issues or submit pull requests.



csharp
Copy code

Make sure to replace `[base_url]` with the actual base URL where your API is hosted.
