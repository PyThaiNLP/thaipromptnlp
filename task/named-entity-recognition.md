# Thai named-entity recognition

You can do Thai named-entity recognition in Llama 3 by the prompt:

**system prompt**

> You are Thai linguist that know about Thai language. Your job are annotate the named-entity recognition from text in CoNLL-U Format by the tag; Person for name person, ORG for organization.

Example:

```
> บริษัท ไอช้า จำกัด เปิดตัวสินค้าไอทีใหม่นำโดย นางบุญสวย อยู่มาดี ประธานบริษัททำการเปิดตัวสินค้า
<
Here is the annotated text in CoNLL-U format:

1	บริษัท	_	ORG	_	_
2	ไอช้า	_	ORG	_	_
3	จำกัด	_	ORG	_	_
4	เปิดตัวสินค้า	_	O	_	_
5	ไอที	_	O	_	_
6	ใหม่	_	O	_	_
7	นำโดย	_	O	_	_
8	นางบุญสวย	_	Person	_	_
9	อยู่มาดี	_	Person	_	_
10	ประธานบริษัท	_	O	_	_
11	ทำการ	_	O	_	_
12	เปิดตัวสินค้า	_	O	_	_

Note:

* ORG: Organization (บริษัท ไอช้า จำกัด)
* Person: Person's name (นางบุญสวย อยู่มาดี)
* O: Not a named entity (other words in the sentence)
```

Url: [https://hf.co/chat/r/pRaqhzv](https://hf.co/chat/r/pRaqhzv)
