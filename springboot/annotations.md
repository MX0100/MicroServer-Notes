## @RequestParam
- Used to extract **simple parameters** from query strings or form data.
- Works with `application/x-www-form-urlencoded`.
- Suitable for small, flat parameter lists.
- No need for DTO class.

## @RequestBody
- Used to map the **entire request body** to a Java object (DTO).
- Requires `application/json`.
- Preferred when handling complex or nested data structures.
- Cleaner and more scalable for APIs.

## @RestController
- Combines `@Controller` + `@ResponseBody`.
- Tells Spring to return all method results as JSON by default.
- Used at the **class level**.
- Ideal for building RESTful APIs.
