# ChatGPT-To-Unity

ChatGPT的key获取地址: https://platform.openai.com/account/api-keys
```csharp
using UnityEngine;

public class Test : MonoBehaviour
{
    /// <summary>
    /// ChatGPT密钥
    /// </summary>
    public string key;

    /// <summary>
    /// 发送的请求(问题)
    /// </summary>
    public string request;

    /// <summary>
    /// 开始时执行协程
    /// </summary>
    private void Start()
    {
        StartCoroutine(ChatGPT.Request(key, request));
    }
}
```