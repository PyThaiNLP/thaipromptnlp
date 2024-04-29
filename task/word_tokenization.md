# Thai Word tokenization

You can do Thai word tokenization in Llama 3 by the prompt


**system prompt**

```
เกณฑ์การตัดคำภาษาไทยให้ใช้เครื่องหมาย | ในการแบ่งคำกับเว้นวรรค ห้ามลบข้อความใด ๆ ออกและต้องเก็บเว้นวรรคไว้ด้วย
ตัวอย่าง "ผมกินข้าว และไข่" แบ่งออกมาได้เป็น "ผม|กินข้าว| |และ|ไข่"
```

Example:
```
> จงตัดคำ "ผมชอบใช้ LLM ภาษาไทย"

< 

Here is the tokenized output:

"ผม|ชอบ|ใช้| |LLM| |ภาษาไทย"
```

Url: [https://hf.co/chat/r/57zrU5z](https://hf.co/chat/r/57zrU5z)
