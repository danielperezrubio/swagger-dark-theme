# Swagger Dark Theme

A dark theme for swagger docs

## Fastapi example

```python
app = FastAPI(docs_url=None)

@app.get("/docs", include_in_schema=False)
async def custom_swagger_ui_html():
    return get_swagger_ui_html(
        openapi_url=app.openapi_url,
        title=f"{app.title} - Swagger UI",
        swagger_css_url="https://cdn.jsdelivr.net/gh/danielperezrubio/swagger-dark-theme@main/assets/swagger-ui.min.css",
    )
```

**CDN link**

```
https://cdn.jsdelivr.net/gh/danielperezrubio/swagger-dark-theme@main/assets/swagger-ui.min.css
```
