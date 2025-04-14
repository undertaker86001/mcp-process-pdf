
## mcp-process-pdf

PDF 文档处理工具

##  主要特性

- 文本提取：多语言支持，保留格式。
- 图片处理：提取与优化。
- 表格识别：结构化数据输出。
- 智能分类：基于深度学习。
- 相似度分析：跨语言比较。
- 多语言支持：100+ 种语言。

##  系统要求

- ** 硬件**：2 核 CPU，4GB 内存。
- **⚙ 软件**：Python 3.10+，可选 CUDA 支持。

##  快速开始

1. ️ 克隆仓库并进入目录：
   ```bash
   git clone https://github.com/saury1120/pdf-mcp.git
   cd pdf-mcp
   ```
2.  创建虚拟环境并安装依赖：
   ```bash
   uv venv
   source .venv/bin/activate
   uv pip install -r requirements.txt
   ```
3.  启动服务：
   ```bash
   uv run pdf_reader

   
### Claude Desktop 配置
1. 找到配置文件：
   - macOS: `~/Library/Application Support/Claude/claude_desktop_config.json`
   - Windows: `%AppData%/Claude/claude_desktop_config.json`
2. 添加以下配置：
```json
{
    "mcpServers": {
        "pdf_reader": {
            "command": "uv",
            "args": [
                "--directory",
                "/path/to/pdf-mcp",  # 替换为实际路径
                "run",
                "pdf_reader"
            ]
        }
    }
}
 ```

