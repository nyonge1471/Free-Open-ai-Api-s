
---

## FREE OPEN-AI API'S

![GitHub Animation](https://docs.aimlapi.com/~gitbook/image?url=https%3A%2F%2F3927338786-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FROMd1X5PuqtikJ48n2N9%252Fuploads%252F88Qvg2NsIg7zP5c5e9ON%252Fimage.png%3Falt%3Dmedia%26token%3Dc042ac97-4bcf-478c-a269-1af5d30cee66&width=768&dpr=1&quality=100&sign=25f65aaa&sv=1)

This documentation provides a comprehensive guide to getting started with the AI/ML API, including generating an API key, configuring the base URL, making your first API call, and running a simple Python application. ```markdown
# MY Documentation-----STAR MY PROJECT IF YOU FIND IT USEFULL

## Profile Update
I have changed my GitHub profile from **dan1471** to **nyonge**.

---

## Generating an API Key

### What is an API Key?
To use the AI/ML API, you need to create an account and generate an API key. Follow these steps:

1. **Create an Account**: Visit the AI/ML API website and create an account.
2. **Generate an API Key**: After logging in, navigate to your account dashboard and generate your API key. Ensure that the key is enabled on the UI.

### Your API Key
Make sure to keep your API key secure and do not share it publicly.

---

## Configure Base URL
**https://api.aimlapi.com**
### What is a Base URL?
Depending on your environment and application, you will set the base URL differently. Below is a universal string that you can use to access our API. Copy it or return here later when you are ready with your environment or app.

The AI/ML API supports both versioned and non-versioned URLs, providing flexibility in your API requests. You can use either of the following formats:

- `https://api.aimlapi.com`
- `https://api.aimlapi.com/v1`

Using versioned URLs can help ensure compatibility with future updates and changes to the API. It is recommended to use versioned URLs for long-term projects to maintain stability.

---

## Making Your First API Call

Based on your environment, you will call our API differently. Below are two common ways to call our API using two popular programming languages: Python and NodeJS.

In the examples below, we use the OpenAI SDK. This is possible due to our compatibility with most OpenAI APIs, but this is just one approach. You can use our API without this SDK with raw HTTP queries.

### Code Explanation
Both examples are written in different programming languages, but despite that, they look very similar. Let's break down the code step by step and see what's going on.

1. **Import the OpenAI SDK**:
    ```python
    from openai import OpenAI
    ```

2. **Initialize Variables**:
    ```python
    base_url = "https://api.aimlapi.com/v1"
    api_key = "my_key"
    system_prompt = "You are a travel agent. Be descriptive and helpful."
    user_prompt = "Tell me about San Francisco"
    ```

3. **Create an Instance of the OpenAI SDK**:
    ```python
    api = OpenAI(api_key=api_key, base_url=base_url)
    ```

4. **Send a Request**:
    ```python
    completion = api.chat.completions.create(
        model="mistralai/Mistral-7B-Instruct-v0.2",
        messages=[
            {"role": "system", "content": system_prompt},
            {"role": "user", "content": user_prompt},
        ],
        temperature=0.7,
        max_tokens=256,
    )
    ```

5. **Get the Response**:
    ```python
    response = completion.choices[0].message.content
    ```

6. **Print the Conversation**:
    ```python
    print("User  :", user_prompt)
    print("AI:", response)
    ```

### Future Steps
- Know more about OpenAI SDK inside AI/ML API.

---

## Example Using Python

Let's start from the very beginning. We assume you already installed Python (with venv). If not, here’s a guide for beginners.

1. **Create a New Folder for the Test Project**:
    ```bash
    mkdir ./aimlapi-welcome
    cd ./aimlapi-welcome
    ```

2. **(Optional)** If you use an IDE, open the created folder as a workspace. For example, in VSCode:
    ```bash
    code .
    ```

3. **Run a Terminal Inside the Created Folder and Create a Virtual Environment**:
    ```bash
    python3 -m venv ./.venv
    ```

4. **Activate the Created Virtual Environment**:
    - **Linux / Mac**:
        ```bash
        source ./.venv/bin/activate
        ```
    - **Windows**:
        ```bash
        .\.venv\Scripts\activate
        ```

5. **Install Required Dependencies**:
    ```bash
    pip install openai
    ```

6. **Create a New File and Name It `travel.py`**:
    ```bash
    touch travel.py
    ```

7. **Paste the Following Content Inside `travel.py`** and replace `my_key` with your API key:
    ```python
    from open ```python
    from openai import OpenAI

    base_url = "https://api.aimlapi.com/v1"
    api_key = "my_key"
    system_prompt = "You are a travel agent. Be descriptive and helpful."
    user_prompt = "Tell me about San Francisco"

    api = OpenAI(api_key=api_key, base_url=base_url)

    def main():
        completion = api.chat.completions.create(
            model="mistralai/Mistral-7B-Instruct-v0.2",
            messages=[
                {"role": "system", "content": system_prompt},
                {"role": "user", "content": user_prompt},
            ],
            temperature=0.7,
            max_tokens=256,
        )

        response = completion.choices[0].message.content

        print("User   :", user_prompt)
        print("AI:", response)

    if __name__ == "__main__":
        main()
    ```

8. **Run the Application**:
    ```bash
    python3 ./travel.py
    ```

**If you have done everything correctly, you will see the following output:**
--:User Tell me about San Francisco AI: San Francisco, located in northern California, USA, is a vibrant and culturally rich city known for its iconic landmarks, beautiful vistas, and diverse neighborhoods. It's a popular tourist destination famous for its iconic Golden Gate Bridge, which spans the entrance to the San Francisco Bay, and the iconic Alcatraz Island, home to the infamous federal prison.

The city's famous hills offer stunning views of the bay and the cityscape. Lombard Street, the "crookedest street in the world," is a must-see attraction, with its zigzagging pavement and colorful gardens. Ferry Building Marketplace is a great place to explore local food and artisanal products, and the Pier 39 area is home to sea lions, shops, and restaurants.

San Francisco's diverse neighborhoods each have their unique character. The historic Chinatown is the oldest in North America, while the colorful streets of the Mission District are known for their murals and Latin American culture. The Castro District is famous for its LGBTQ+ community and vibrant nightlife.--
  
---

## GitHub Animations

![my pltform](https://docs.aimlapi.com/~gitbook/image?url=https%3A%2F%2F3927338786-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FROMd1X5PuqtikJ48n2N9%252Fuploads%252F88Qvg2NsIg7zP5c5e9ON%252Fimage.png%3Falt%3Dmedia%26token%3Dc042ac97-4bcf-478c-a269-1af5d30cee66&width=768&dpr=1&quality=100&sign=25f65aaa&sv=1)

**This documentation provides a comprehensive guide to getting started with the FREE API, including generating an API key, configuring the base URL, making your first API call, and running YOUR PROJECTS**.
