
OpenAI 在 [6 月发布测试版](https://github.com)\[1]后[发布了其官方 .NET 库的稳定版本](https://github.com)\[2]。它以 [NuGet 包](https://github.com)\[3]的形式提供，支持 GPT\-4o 和 GPT\-4o mini 等最新模型，以及完整的 OpenAI REST API。该版本包括同步和异步 API、流式聊天完成以及用于提高 API 一致性的关键性更改。开发人员可以扩展该库，并在支持 .NET Standard 2\.0 的所有 .NET 平台上使用它。

Microsoft 的 .NET 团队在 10 月 1 日的[一篇文章](https://github.com)\[2]中说。“今天，我们很高兴地宣布，[适用于 .NET 的官方 OpenAI 库](https://github.com)\[3]的稳定版本现已上线。此版本可确保开发人员在其 .NET 应用程序中使用 OpenAI 和 Azure OpenAI 服务时获得流畅可靠的集成体验。

其目的是提供工具来简化将 OpenAI 的尖端模型集成到 .NET 应用程序中的过程，为开发人员提供简化的体验，用 Microsoft 的话来说，其功能包括：

* **完整的 OpenAI REST API 支持：**包括 Assistants v2 和 Chat Completions，可实现灵活和高级的交互。
* **支持最新型号：**OpenAI 的最新旗舰模型，包括 GPT\-4o、GPT\-4o mini、o1\-preview 和 o1\-mini，得到全面支持，确保开发人员能够获得尖端的 AI 功能。
* **扩展：**该库在设计时考虑了可扩展性，允许社区在其上构建其他库。
* **同步和异步 API：**这确保了开发人员可以根据其应用程序的需求灵活地使用同步或异步模式。
* **流式补全：**通过 IAsyncEnumerable 访问流式补全，从而提供更动态的交互模型。
* **代码质量改进：**在整个测试周期中，根据社区反馈进行了大量改进。
* **.NET Standard 2\.0 兼容性：**此库以 C\# 编写，支持实现 .NET Standard 2\.0 的所有 .NET 变体，确保与最新的 .NET 平台兼容。

对于从 2\.0\.0\-beta.\* 版本升级的开发人员，引入了几项重大更改，以提高 API 的一致性和可用性：

* `ChatMessageContent`现在将内容部分封装在`ChatMessage` 、`ChatCompletion``Streaming` 和 `ChatCompletionUpdate`中。
* 函数参数现在表示为多个区域，包括`BinaryData``ChatToolCall` 和`StreamingChatToolCallUpdate` 。
* 应用了多种重命名约定：已重命名为`ApplicationId` 、`UserAgentApplicationId` 为 `FileClient`和`OpenAIFileClient` 为 `ModelClient ，OpenAIModelClient`等。
* 已弃用的构造函数和方法已替换为新选项`ChatFunctionChoice`，例如将 `Auto`和 `None`替换为`CreateAutoChoice()` 和`CreateNoneChoice()` 。

其 <https://github.com/shanyou/p/18238209>:[milou加速器](https://xinminxuehui.org)- \[2]官方 .NET 库的稳定版本:[https://devblogs.microsoft.com/dotnet/announcing\-the\-stable\-release\-of\-the\-official\-open\-ai\-library\-for\-dotnet/](https://devblogs.microsoft.com/dotnet/announcing-the-stable-release-of-the-official-open-ai-library-for-dotnet/ "https://devblogs.microsoft.com/dotnet/announcing-the-stable-release-of-the-official-open-ai-library-for-dotnet/")
- \[3]适用于 .NET 的官方 OpenAI 库:[https://www.nuget.org/packages/OpenAI/2\.0\.0](https://www.nuget.org/packages/OpenAI/2.0.0 "https://www.nuget.org/packages/OpenAI/2.0.0")
- \[4]GitHub 存储库:[https://github.com/openai/openai\-dotnet](https://github.com/openai/openai-dotnet "https://github.com/openai/openai-dotnet")
- \[5]Azure SDK:[https://github.com/Azure/azure\-sdk\-for\-net](https://github.com/Azure/azure-sdk-for-net "https://github.com/Azure/azure-sdk-for-net")



