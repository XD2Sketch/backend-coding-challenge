# Backend Coding Challenge

The goal of this coding challenge is to write a service that fetches data from the Figma API for a given Figma Design and stores it as a JSON file to S3.

Please try to not spend more than 4 hours on the challenge.

### Requirements:
- Users should be able to submit a Figma File URL and the service downloads the JSON and stores it to S3
  -  Figma URL format: `https://figma.com/file/FILE_ID` or `https://www.figma.com/file/FILE_ID`
- Users should be able to download the JSON from the S3 bucket afterwards

Test Figma Design: https://www.figma.com/file/7jRyj8dzankbyraCDBVwBM

Documentation: https://www.figma.com/developers/api#get-files-endpoint

Curl Request Example:

```bash
curl -H 'X-FIGMA-TOKEN: YOUR_TOKEN' 'https://api.figma.com/v1/files/7jRyj8dzankbyraCDBVwBM'
```

Example Response from the Figma API:

```json
{
  "document": {
    "id": "0:0",
    "name": "Document",
    "type": "DOCUMENT",
    "children": [
      {
        "id": "0:1",
        "name": "Page 1",
        "type": "CANVAS",
        "children": [
          {
            ...
          }
        ]
      }
    ]
  }
}
```

#### Technical Recommendations:
- Use TypeScript, NodeJs
- Usage of modern js functionality (ES6+)
- Documentation
- Clean commits (consider Conventional Commit Messages)
- Clean code (linting, ...)
- Fastify, Express, Nest
- Defined REST endpoints
- Schema Validation
- Some Tests
- Async/Await
- Logging

#### Nice to have:
- Gitflow Branch Naming

#### Stuff we will pay attention to:
- How you split your code
- Code repetitions and reusability (keep your code DRY and simple KISS)
- How and where you put your business logic
- Working in accordance with good practices in general
- Handling unexpected errors or potential exceptions
