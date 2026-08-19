```rust
    async fn solve_captcha(&self, captcha_data: &str) -> VtopResult<String> {
        let url_safe_encoded = URL_SAFE.encode(captcha_data.as_bytes());
        let captcha_url = format!("https://cap.va.synaptic.gg/captcha");

        #[derive(Serialize)]
        struct PostData {
            imgstring: String,
        }

        let client_for_post = reqwest::Client::new();
        let post_data = PostData {
            imgstring: url_safe_encoded,
        };
        let response = client_for_post
            .post(captcha_url)
            .json(&post_data)
            .send()
            .await
            .map_err(|_| VtopError::NetworkError)?;

        if !response.status().is_success() {
            return Err(VtopError::NetworkError);
        }
        response.text().await.map_err(|_| VtopError::NetworkError)
    }
```
> Lets not do this
### Get Login request to work
> Either rewrite 
- [ ] Username, Password, and Captcha thing
- [ ] Cookies ???
