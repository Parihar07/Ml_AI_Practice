# Advanced Problem 1: System Design - URL Shortener

## Difficulty Level
Advanced

## Problem Description
Design a URL shortener service like bit.ly or TinyURL. You need to:
1. Convert long URLs into short, unique URLs
2. Retrieve the original URL from a short URL
3. Handle high traffic and concurrent requests

## Constraints
- Support 100 billion URLs
- Short URL length: ~6 characters
- Average retrieval latency: < 100ms
- 99.9% availability
- No automatic expiration (URLs live forever)

## System Requirements
- Read-heavy system (100:1 read-write ratio)
- Generate unique short codes
- Support distributed system
- Handle concurrent access

## Design Considerations
### Components to Design
1. **Encoding Strategy**: How to convert long URLs to short codes
2. **Data Storage**: Database schema and indexing strategy
3. **API Design**: Endpoint specifications
4. **Scalability**: How to handle growth
5. **Caching**: Strategy for frequently accessed URLs
6. **Reliability**: Handling failures and consistency

## Example Flow

### Create Short URL
```
POST /shorten
{
  "long_url": "https://www.example.com/page/with/very/long/url"
}

Response:
{
  "short_url": "https://tinyurl.com/abc123",
  "long_url": "https://www.example.com/page/with/very/long/url"
}
```

### Retrieve Original URL
```
GET /expand?short_url=https://tinyurl.com/abc123

Response:
{
  "long_url": "https://www.example.com/page/with/very/long/url"
}
```

## Key Concepts
- Hash functions and encoding
- Database design (SQL vs NoSQL)
- Caching strategies (Redis, Memcached)
- Load balancing
- API design principles
- Distributed systems

## Evaluation Criteria
- [ ] Clear understanding of the problem
- [ ] Well-designed API
- [ ] Efficient encoding scheme
- [ ] Scalable architecture
- [ ] Handles edge cases
- [ ] Explains trade-offs
- [ ] Addresses failures and recovery

## Discussion Topics
- Why did you choose this encoding?
- SQL or NoSQL? Why?
- How would you handle collisions?
- How to ensure unique short codes globally?
- What caching strategy would you use?
- How to handle system failures?
- Scaling considerations?

---
**Difficulty:** Hard | **Time Estimate:** 60+ minutes  
**Category:** System Design, Architecture
