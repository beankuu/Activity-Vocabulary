[목차로 돌아가기](ActivityVocabularyContents.md)

## 4. [속성 (Properties)](ActivityVocabularyContents.md)

Base URI: `https://www.w3.org/ns/activitystreams#`.

기반 URI: `https://www.w3.org/ns/activitystreams#`.

The common properties include:

일반적인 속성들은 다음과 같습니다:

 [actor](#class-actor) \|
 [attachment](#class-attachment) \|
 [attributedTo](#class-attributedto) \|
 [audience](#class-audience) \|
 [bcc](#class-bcc) \|
 [bto](#class-bto) \|
 [cc](#class-cc) \|
 [context](#class-context) \|
 [current](#class-current) \|
 [first](#class-first) \|
 [generator](#class-generator) \|
 [icon](#class-icon) \|
 [id](#class-id) \|
 [image](#class-image) \|
 [inReplyTo](#class-inreplyto) \|
 [instrument](#class-instrument) \|
 [last](#class-last) \|
 [location](#class-location) \|
 [items](#class-items) \|
 [oneOf](#class-oneof) \|
 [anyOf](#class-anyof) \|
 [closed](#class-closed) \|
 [origin](#class-origin) \|
 [next](#class-next) \|
 [object](ActivityVocabularyChapter2.md#class-object) \|
 [prev](#class-prev) \|
 [preview](#class-preview) \|
 [result](#class-result) \|
 [replies](#class-replies) \|
 [tag](#class-tag) \|
 [target](#class-target) \|
 [to](#class-to) \|
 [type](#class-type) \|
 [url](#class-url) \|
 [accuracy](#class-accuracy) \|
 [altitude](#class-altitude) \|
 [content](#class-content) \|
 [name](#class-name) \|
 [duration](#class-duration) \|
 [height](#class-height) \|
 [href](#class-href) \|
 [hreflang](#class-hreflang) \|
 [partOf](#class-partof) \|
 [latitude](#class-latitude) \|
 [longitude](#class-longitude) \|
 [mediaType](#class-mediatype) \|
 [endTime](#class-endtime) \|
 [published](#class-published) \|
 [startTime](#class-starttime) \|
 [radius](#class-radius) \|
 [rel](#class-rel) \|
 [startIndex](#class-startindex) \|
 [summary](#class-summary) \|
 [totalItems](#class-totalitems) \|
 [units](#class-units) \|
 [updated](#class-updated) \|
 [width](#class-width) \|
 [subject](#class-subject) \|
 [relationship](#class-relationship) \|
 [describes](#class-describes) \|
 [formerType](#class-formertype) \|
 [deleted](#class-deleted)

The "Domain" indicates the type of Object the property term applies to. The "Range" indicates the type of value the property term can have. Certain properties are marked as a "Subproperty Of" another term, meaning that the term is a specialization of the referenced term. For instance, [actor](#class-actor) is a subproperty of [attributedTo](#class-attributedto). Properties marked as being "Functional" can have only one value. Items not marked as "Functional" can have multiple values.

"도메인(Domain)"은 속성 용어가 적용되는 객체의 타입을 나타냅니다. "범위(Range)"는 속성 용어가 가질수 있는 값의 타입을 나타냅니다. 특정 속성은 다른 용어의 "하위속성(Subproperty)"으로 표시됩니다. 즉, 해당 용어는 참조된 용어의 특수화된 경우입니다. 예를 들어 [actor](#class-actor)는 [attributedTo](#class-attributedto)의 하위 속성입니다. "기능적(Functional)"으로 표시되어 있는 속성은 하나의 값만 가질수도 있습니다. "기능적(Functional)"으로 표시되지 않은 항목은 여러개의 값을 가질 수 있습니다.

#### [Class] [id](#4-속성-properties)

Description| |
--|--
URI: | `@id`
Notes: | Provides the globally unique identifier for an [Object](ActivityVocabularyChapter2.md#class-object) or [Link](ActivityVocabularyChapter2.md#class-link).
Domain: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)
Range: | `anyURI`
Functional: | True

설명| |
--|--
URI: | `@id`
비고: | [Object](ActivityVocabularyChapter2.md#class-object)나 [Link](ActivityVocabularyChapter2.md#class-link)에 대한 전역 고유 식별자를 제공합니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)
범위: | `anyURI`
기능적: | True

>Example 61

>예시 61
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "name": "Foo",
>  "id": "http://example.org/foo"
>}
>```

#### [Class] [type](#4-속성-properties)

Description| |
--|--
URI: | `@type`
Notes: | Identifies the [Object](ActivityVocabularyChapter2.md#class-object) or [Link](ActivityVocabularyChapter2.md#class-link) type. Multiple values may be specified.
Domain: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)
Range: | `anyURI`

설명| |
--|--
URI: | `@type`
비고: | [Object](ActivityVocabularyChapter2.md#class-object)나 [Link](ActivityVocabularyChapter2.md#class-link) 타입을 식별합니다. 다중 값을 지정 할 수도 있습니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)
범위: | `anyURI`

[//Comment]: # "Object과 Link가 대문자로 시작되었고, 차후 문장에서 사용하지 않았음으로 원문으로 냅두었습니다."

>Example 62

>예시 62
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "A foo",
>  "type": "http://example.org/Foo"
>}
>```

#### [Class] [actor](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#actor`
Notes: | Describes one or more entities that either performed or are expected to perform the activity. Any single activity can have multiple `actor`s. The `actor` *MAY* be specified using an indirect [Link](ActivityVocabularyChapter2.md#class-link).
Domain: | [Activity](ActivityVocabularyChapter2.md#class-activity)
Range: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)
Subproperty Of: | [attributedTo](#class-attributedto)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#actor`
비고: | 액티비티를 수행했거나 수행할 것으로 예상되는 하나 이상의 개체들을 표현합니다. 단일 액티비티에는 여러 `actor`가 있을 수 있습니다. `actor`는 간접 [Link](ActivityVocabularyChapter2.md#class-link)를 사용하여 지정 *할 수도* 있습니다.
도메인: | [Activity](ActivityVocabularyChapter2.md#class-activity)
범위: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)
하위속성: | [attributedTo](#class-attributedto)

>Example 63
>
>```json
>{
>  "summary": "Sally offered the Foo object",
>}
>```

>예시 63
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally는 Foo 객체를 제공했습니다",
>  "type": "Offer",
>  "actor": "http://sally.example.org",
>  "object": "http://example.org/foo"
>}
>```

>Example 64
>
>```json
>{
>  "summary": "Sally offered the Foo object",
>}
>```

>예시 64
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally는 Foo 객체를 제공했습니다",
>  "type": "Offer",
>  "actor": {
>    "type": "Person",
>    "id": "http://sally.example.org",
>    "summary": "Sally"
>  },
>  "object": "http://example.org/foo"
>}
>```

>Example 65
>
>```json
>{
>  "summary": "Sally and Joe offered the Foo object",
>}
>```

>예시 65
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally와 Joe는 Foo 객체를 제공했습니다",
>  "type": "Offer",
>  "actor": [
>    "http://joe.example.org",
>    {
>      "type": "Person",
>      "id": "http://sally.example.org",
>      "name": "Sally"
>    }
>  ],
>  "object": "http://example.org/foo"
>}
>```

#### [Class] [attachment](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#attachment`
Notes: | Identifies a resource attached or related to an object that potentially requires special handling. The intent is to provide a model that is at least semantically similar to attachments in email.
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#attachment`
비고: | 특별한 처리가 필요할수도 있는 개체에 첨부(attached)되었거나 관련된 리소스를 식별합니다. 이메일의 첨부파일과 의미적으로 유사한 모델을 제공하는것 이 목적입니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

>Example 66
>
>```json
>{
>  "name": "Have you seen my cat?",
>      "content": "This is what he looks like.",
>}
>```

>예시 66
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Note",
>  "name": "제 고양이를 보신적이 있나요?",
>  "attachment": [
>    {
>      "type": "Image",
>      "content": "이렇게 생겼어요.",
>      "url": "http://example.org/cat.jpeg"
>    }
>  ]
>}
>```

#### [Class] [attributedTo](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#attributedTo`
Notes: | Identifies one or more entities to which this object is attributed. The attributed entities might not be Actors. For instance, an object might be attributed to the completion of another activity.
Domain: | [Link](ActivityVocabularyChapter2.md#class-link) \| [Object](ActivityVocabularyChapter2.md#class-object)
Range: | [Link](ActivityVocabularyChapter2.md#class-link) \| [Object](ActivityVocabularyChapter2.md#class-object)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#attributedTo`
비고: | 이 객체가 속하는(attributed) 하나 이상의 개체들을 식별합니다. 속하는 개체들은 액터(Actor)가 아닐 수도 있습니다. 예를 들어, 어떤 객체는 '다른 액티비티가 완료되는것' 에 속할 수도 있습니다.
도메인: | [Link](ActivityVocabularyChapter2.md#class-link) \| [Object](ActivityVocabularyChapter2.md#class-object)
범위: | [Link](ActivityVocabularyChapter2.md#class-link) \| [Object](ActivityVocabularyChapter2.md#class-object)

>Example 67
>
>```json
>{
>  "name": "My cat taking a nap",
>}
>```

>예시 67
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Image",
>  "name": "낮잠을 자고 있는 내 고양이",
>  "url": "http://example.org/cat.jpeg",
>  "attributedTo": [
>    {
>      "type": "Person",
>      "name": "Sally"
>    }
>  ]
>}
>```

>Example 68
>
>```json
>{
>  "name": "My cat taking a nap",
>}
>```

>예시 68
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Image",
>  "name": "낮잠을 자고 있는 내 고양이",
>  "url": "http://example.org/cat.jpeg",
>  "attributedTo": [
>    "http://joe.example.org",
>    {
>      "type": "Person",
>      "name": "Sally"
>    }
>  ]
>}
>```

#### [Class] [audience](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#audience`
Notes: | Identifies one or more entities that represent the total population of entities for which the object can considered to be relevant.
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#audience`
비고: | 해당 객체와 관련있는 것으로 간주되는, 총 개체수를 나타내는 하나 이상의 개체들을 식별합니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

>Example 69
>
>```json
>{
>  "name": "Holiday announcement",
>  "content": "Thursday will be a company-wide holiday. Enjoy your day off!",
>    "name": "ExampleCo LLC"
>}
>```

>예시 69
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "name": "휴무일 발표",
>  "type": "Note",
>  "content": "목요일은 회사 전체 휴무일입니다. 휴일을 즐기세요!",
>  "audience": {
>    "type": "http://example.org/Organization",
>    "name": "(유) ExampleCo"
>  }
>}
>```

#### [Class] [bcc](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#bcc`
Notes: | Identifies one or more Objects that are part of the private secondary audience of this Object.
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#bcc`
비고: | 이 객체(Object)의 2차적 비공개 청자에 속하는 하나 이상의 Objects를 식별합니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

>Example 70
>
>```json
>{
>  "summary": "Sally offered a post to John",
>}
>```

>예시 70
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally는 John에게 게시물을 제공했습니다",
>  "type": "Offer",
>  "actor": "http://sally.example.org",
>  "object": "http://example.org/posts/1",
>  "target": "http://john.example.org",
>  "bcc": [ "http://joe.example.org" ]
>}
>```

#### [Class] [bto](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#bto`
Notes: | Identifies an Object that is part of the private primary audience of this Object.
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#bto`
비고: | 이 객체(Object)의 주요 비공개 청자의 일부인 Object를 식별합니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

>Example 71
>
>```json
>{
>  "summary": "Sally offered a post to John",
>}
>```

>예시 71
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally는 John에게 게시물을 제공했습니다",
>  "type": "Offer",
>  "actor": "http://sally.example.org",
>  "object": "http://example.org/posts/1",
>  "target": "http://john.example.org",
>  "bto": [ "http://joe.example.org" ]
>}
>```

#### [Class] [cc](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#cc`
Notes: | Identifies an Object that is part of the public secondary audience of this Object.
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#cc`
비고: | 이 객체(Object)의 2차적 공개 청자의 일부인 Object를 식별합니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

>Example 72
>
>```json
>{
>  "summary": "Sally offered a post to John",
>}
>```

>예시 72
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally는 John에게 게시물을 제공했습니다",
>  "type": "Offer",
>  "actor": "http://sally.example.org",
>  "object": "http://example.org/posts/1",
>  "target": "http://john.example.org",
>  "cc": [ "http://joe.example.org" ]
>}
>```

#### [Class] [context](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#context`
Notes: | Identifies the context within which the object exists or an activity was performed.</br> The notion of "context" used is intentionally vague. The intended function is to serve as a means of grouping objects and activities that share a common originating context or purpose. An example could be all activities relating to a common project or event.
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#context`
비고: | 개체가 존재하거나 액티비티가 실행된 된 컨텍스트(context)를 식별합니다. </br> "컨텍스트"라는 개념은 의도적으로 모호하게 사용되었습니다. 의도되었던 기능은 공통적인 컨텍스트 또는 목적을 공유하는 객체와 액티비티를 그룹화하는 수단으로 사용하려는 것입니다. 예시로는 일반적인 프로젝트 또는 이벤트와 관련된 모든 액티비티들 입니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

>Example 73
>
>```json
>{
>  "summary": "Activities in context 1",
>}
>```

>예시 73
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "컨텍스트 1 안의 액티비티들",
>  "type": "Collection",
>  "items": [
>    {
>      "type": "Offer",
>      "actor": "http://sally.example.org",
>      "object": "http://example.org/posts/1",
>      "target": "http://john.example.org",
>      "context": "http://example.org/contexts/1"
>    },
>    {
>      "type": "Like",
>      "actor": "http://joe.example.org",
>      "object": "http://example.org/posts/2",
>      "context": "http://example.org/contexts/1"
>    }
>  ]
>}
>```

#### [Class] [current](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#current`
Notes: | In a paged Collection, indicates the page that contains the most recently updated member items.
Domain: | [Collection](ActivityVocabularyChapter2.md#class-collection)
Range: | [CollectionPage](ActivityVocabularyChapter2.md#class-collectionpage) \| [Link](ActivityVocabularyChapter2.md#class-link)
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#current`
비고: | 페이징 된 컬렉션에서 가장 최근에 업데이트된 구성원의 항목이 포함된 페이지를 나타냅니다.
도메인: | [Collection](ActivityVocabularyChapter2.md#class-collection)
범위: | [CollectionPage](ActivityVocabularyChapter2.md#class-collectionpage) \| [Link](ActivityVocabularyChapter2.md#class-link)
기능적: | True

>Example 74
>
>```json
>{
>  "summary": "Sally's blog posts",
>}
>```

>예시 74
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally의 블로그 포스트들",
>  "type": "Collection",
>  "totalItems": 3,
>  "current": "http://example.org/collection",
>  "items": [
>    "http://example.org/posts/1",
>    "http://example.org/posts/2",
>    "http://example.org/posts/3"
>  ]
>}
>```

>Example 75
>
>```json
>{
>  "summary": "Sally's blog posts",
>    "summary": "Most Recent Items",
>}
>```

>예시 75
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally의 블로그 포스트들",
>  "type": "Collection",
>  "totalItems": 3,
>  "current": {
>    "type": "Link",
>    "summary": "가장 최근의 항목들",
>    "href": "http://example.org/collection"
>  },
>  "items": [
>    "http://example.org/posts/1",
>    "http://example.org/posts/2",
>    "http://example.org/posts/3"
>  ]
>}
>```

#### [Class] [first](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#first`
Notes: | In a paged Collection, indicates the furthest preceeding page of items in the collection.
Domain: | [Collection](ActivityVocabularyChapter2.md#class-collection)
Range: | [CollectionPage](ActivityVocabularyChapter2.md#class-collectionpage) \| [Link](ActivityVocabularyChapter2.md#class-link)
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#first`
비고: | 페이징 된 컬렉션에서 컬렉션의 가장 앞에있는 페이지를 나타냅니다.
도메인: | [Collection](ActivityVocabularyChapter2.md#class-collection)
범위: | [CollectionPage](ActivityVocabularyChapter2.md#class-collectionpage) \| [Link](ActivityVocabularyChapter2.md#class-link)
기능적: | True

>Example 76
>
>```json
>{
>  "summary": "Sally's blog posts",
>}
>```

>예시 76
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally의 블로그 포스트들",
>  "type": "Collection",
>  "totalItems": 3,
>  "first": "http://example.org/collection?page=0"
>}
>```

>Example 77
>
>```json
>{
>  "summary": "Sally's blog posts",
>    "summary": "First Page",
>}
>```

>예시 77
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally의 블로그 포스트들",
>  "type": "Collection",
>  "totalItems": 3,
>  "first": {
>    "type": "Link",
>    "summary": "첫 페이지",
>    "href": "http://example.org/collection?page=0"
>  }
>}
>```

#### [Class] [generator](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#generator`
Notes: | Identifies the entity (e.g. an application) that generated the object.
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#generator`
비고: | 객체를 생성한(generated) 개체(예: 어플리케이션)을 식별합니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

>Example 78
>
>```json
>{
>  "summary": "A simple note",
>  "content": "This is all there is.",
>    "name": "Exampletron 3000"
>}
>```

>예시 78
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "간단한 노트",
>  "type": "Note",
>  "content": "여기 있는게 전부에요.",
>  "generator": {
>    "type": "Application",
>    "name": "예시제조기 3000"
>  }
>}
>```

#### [Class] [icon](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#icon`
Notes: | Indicates an entity that describes an icon for this object. The image should have an aspect ratio of one (horizontal) to one (vertical) and should be suitable for presentation at a small size.
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | [Image](#class-image) \| [Link](ActivityVocabularyChapter2.md#class-link)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#icon`
비고: | 이 객체의 아이콘(icon)을 나타내는 개체를 나타냅니다. 이미지의 가로-세로 비율은 1(수평) 대 1(수직)이여야 하며 작은 크기로 보여주는것에 적합하여야 합니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | [Image](#class-image) \| [Link](ActivityVocabularyChapter2.md#class-link)

>Example 79
>
>```json
>{
>  "summary": "A simple note",
>  "content": "This is all there is.",
>    "name": "Note icon",
>}
>```

>예시 79
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "간단한 노트",
>  "type": "Note",
>  "content": "여기 있는게 전부에요.",
>  "icon": {
>    "type": "Image",
>    "name": "노트 아이콘",
>    "url": "http://example.org/note.png",
>    "width": 16,
>    "height": 16
>  }
>}
>```

>Example 80
>
>```json
>{
>  "summary": "A simple note",
>  "content": "A simple note",
>      "summary": "Note (16x16)",
>      "summary": "Note (32x32)",
>}
>```

>예시 80
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "간단한 노트",
>  "type": "Note",
>  "content": "간단한 노트",
>  "icon": [
>    {
>      "type": "Image",
>      "summary": "노트 (16x16)",
>      "url": "http://example.org/note1.png",
>      "width": 16,
>      "height": 16
>    },
>    {
>      "type": "Image",
>      "summary": "노트 (32x32)",
>      "url": "http://example.org/note2.png",
>      "width": 32,
>      "height": 32
>    }
>  ]
>}
>```

#### [Class] [image](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#image`
Notes: | Indicates an entity that describes an image for this object. Unlike the icon property, there are no aspect ratio or display size limitations assumed.
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | [Image](#class-image) \| [Link](ActivityVocabularyChapter2.md#class-link)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#image`
비고: | 이 객체의 이미지(image)를 기술하는 개체를 나타냅니다. icon속성과 달리 종횡비나 디스클레이에 대한 크기 제한은 없습니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | [Image](#class-image) \| [Link](ActivityVocabularyChapter2.md#class-link)

>Example 81
>
>```json
>{
>  "name": "A simple note",
>  "content": "This is all there is.",
>    "name": "A Cat",
>}
>```

>예시 81
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "name": "간단한 노트",
>  "type": "Note",
>  "content": "여기 있는게 전부에요.",
>  "image": {
>    "type": "Image",
>    "name": "고양이",
>    "url": "http://example.org/cat.png"
>  }
>}
>```

>Example 82
>
>```json
>{
>  "name": "A simple note",
>  "content": "This is all there is.",
>      "name": "Cat 1",
>      "name": "Cat 2",
>}
>```

>예시 82
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "name": "간단한 노트",
>  "type": "Note",
>  "content": "여기 있는게 전부에요.",
>  "image": [
>    {
>      "type": "Image",
>      "name": "고양이 1",
>      "url": "http://example.org/cat1.png"
>    },
>    {
>      "type": "Image",
>      "name": "고양이 2",
>      "url": "http://example.org/cat2.png"
>    }
>  ]
>}
>```

#### [Class] [inReplyTo](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#inReplyTo`
Notes: | Indicates one or more entities for which this object is considered a response.
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#inReplyTo`
비고: | 이 객체를 응답으로 간주하는 하나 이상의 개체를 나타냅니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

>Example 83
>
>```json
>{
>  "name": "A simple note",
>  "content": "This is all there is.",
>    "summary": "Previous note",
>    "content": "What else is there?"
>}
>```

>예시 83
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "간단한 노트",
>  "type": "Note",
>  "content": "여기 있는게 전부에요.",
>  "inReplyTo": {
>    "summary": "이전 노트",
>    "type": "Note",
>    "content": "거기에 더 있나요?"
>  }
>}
>```

>Example 84
>
>```json
>{
>  "summary": "A simple note",
>  "content": "This is all there is.",
>}
>```

>예시 84
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "간단한 노트",
>  "type": "Note",
>  "content": "여기 있는게 전부에요.",
>  "inReplyTo": "http://example.org/posts/1"
>}
>```

#### [Class] [instrument](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#instrument`
Notes: | Identifies one or more objects used (or to be used) in the completion of an [Activity](ActivityVocabularyChapter2.md#class-activity).
Domain: | [Activity](ActivityVocabularyChapter2.md#class-activity)
Range: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#instrument`
비고: | [Activity](ActivityVocabularyChapter2.md#class-activity)가 완료시 사용된 (또는 사용되는) 하나 이상의 객체들을 식별합니다.
도메인: | [Activity](ActivityVocabularyChapter2.md#class-activity)
범위: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

>Example 85
>
>```json
>{
>  "summary": "Sally listened to a piece of music on the Acme Music Service",
>    "name": "Acme Music Service"
>}
>```

>예시 85
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally는 '최상의 음악 서비스'에서 음악을 들었습니다",
>  "type": "Listen",
>  "actor": {
>    "type": "Person",
>    "name": "Sally"
>  },
>  "object": "http://example.org/foo.mp3",
>  "instrument": {
>    "type": "Service",
>    "name": "최상의 음악 서비스"
>  }
>}
>```

#### [Class] [last](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#last`
Notes: | In a paged [Collection](ActivityVocabularyChapter2.md#class-collection), indicates the furthest proceeding page of the collection.
Domain: | [Collection](ActivityVocabularyChapter2.md#class-collection)
Range: | [CollectionPage](ActivityVocabularyChapter2.md#class-collectionpage) \| [Link](ActivityVocabularyChapter2.md#class-link)
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#last`
비고: | 페이징 된 [Collection](ActivityVocabularyChapter2.md#class-collection)에서 컬렉션의 뒷방향으로 가장 멀리있는 페이지를 나타냅니다.
도메인: | [Collection](ActivityVocabularyChapter2.md#class-collection)
범위: | [CollectionPage](ActivityVocabularyChapter2.md#class-collectionpage) \| [Link](ActivityVocabularyChapter2.md#class-link)
기능적: | True

>Example 86
>
>```json
>{
>  "summary": "A collection",
>}
>```

>예시 86
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "컬렉션",
>  "type": "Collection",
>  "totalItems": 3,
>  "last": "http://example.org/collection?page=1"
>}
>```

>Example 87
>
>```json
>{
>  "summary": "A collection",
>    "summary": "Last Page",
>}
>```

>예시 87
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "컬렉션",
>  "type": "Collection",
>  "totalItems": 5,
>  "last": {
>    "type": "Link",
>    "summary": "마지막 페이지",
>    "href": "http://example.org/collection?page=1"
>  }
>}
>```

#### [Class] [location](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#location`
Notes: | Indicates one or more physical or logical locations associated with the object.
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#location`
비고: | 주어진 객체와 관련된 하나 이상의 물리적 또는 논리적인 위치(locations)를 나타냅니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

>Example 88
>
>```json
>{
>    "name": "Over the Arabian Sea, east of Socotra Island Nature Sanctuary",
>}
>```

>예시 88
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Person",
>  "name": "Sally",
>  "location": {
>    "name": "아라비아 해를 넘어서, 소코트라 섬 자연 보호구역의 동쪽",
>    "type": "Place",
>    "longitude": 12.34,
>    "latitude": 56.78,
>    "altitude": 90,
>    "units": "m"
>  }
>}
>```

#### [Class] [items](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#items`
Notes: | Identifies the items contained in a collection. The items might be ordered or unordered.
Domain: | [Collection](ActivityVocabularyChapter2.md#class-collection)
Range: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link) \| Ordered List of [ [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link) ]

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#items`
비고: | 컬렉션에 포함된 항목(items)을 식별합니다. 항목은 정렬되었거나 정렬되지 않았을 수도 있습니다.
도메인: | [Collection](ActivityVocabularyChapter2.md#class-collection)
범위: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link) \| [ [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link) ]의 정렬된 리스트

>Example 89
>
>```json
>{
>  "summary": "Sally's notes",
>      "name": "Reminder for Going-Away Party"
>      "name": "Meeting 2016-11-17"
>}
>```

>예시 89
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally의 노트",
>  "type": "Collection",
>  "totalItems": 2,
>  "items": [
>    {
>      "type": "Note",
>      "name": "송별회 알림"
>    },
>    {
>      "type": "Note",
>      "name": "회의 2016-11-17"
>    }
>  ]
>}
>```

>Example 90
>
>```json
>{
>  "summary": "Sally's notes",
>      "name": "Meeting 2016-11-17"
>      "name": "Reminder for Going-Away Party"
>}
>```

>예시 90
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally의 노트",
>  "type": "OrderedCollection",
>  "totalItems": 2,
>  "orderedItems": [
>    {
>      "type": "Note",
>      "name": "회의 2016-11-17"
>    },
>    {
>      "type": "Note",
>      "name": "송별회 알림"
>    }
>  ]
>}
>```

#### [Class] [oneOf](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#oneOf`
Notes: | Identifies an exclusive option for a Question. Use of `oneOf` implies that the Question can have only a single answer. To indicate that a Question can have multiple answers, use [anyOf](#class-anyof).
Domain: | [Question](ActivityVocabularyChapter3.md#class-question)
Range: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#oneOf`
비고: | 질문(Question)에 대한 독점적인 선택지를 식별합니다. `oneOf`를 사용하는 Question에 대해서는 하나의 답변만 할수 있음을 의미합니다. Question에 여러개의 답변이 있을수 있음을 나타내려면 [anyOf](#class-anyof)를 사용하시길 바랍니다.
도메인: | [Question](ActivityVocabularyChapter3.md#class-question)
범위: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

>Example 91
>
>```json
>{
>  "name": "What is the answer?",
>      "name": "Option A"
>      "name": "Option B"
>}
>```

>예시 91
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Question",
>  "name": "무엇이 정답일까요?",
>  "oneOf": [
>    {
>      "type": "Note",
>      "name": "선택지 A"
>    },
>    {
>      "type": "Note",
>      "name": "선택지 B"
>    }
>  ]
>}
>```

#### [Class] [anyOf](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#anyOf`
Notes: | Identifies an inclusive option for a Question. Use of `anyOf` implies that the Question can have multiple answers. To indicate that a Question can have only one answer, use [oneOf](#class-oneof).
Domain: | [Question](ActivityVocabularyChapter3.md#class-question)
Range: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#anyOf`
비고: | 질문(Question)에 대한 포괄적인 선택지를 식별합니다. `anyOf`를 사용하는 Question에 대해서는 여러개의 답변이 있을수 있음을 나타냅니다. Question에 대해 답변이 단 하나만 존재할수 있음을 나타내려면 [oneOf](#class-oneof)를 사용하시길 바랍니다.
도메인: | [Question](ActivityVocabularyChapter3.md#class-question)
범위: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

>Example 92
>
>```json
>{
>  "name": "What is the answer?",
>      "name": "Option A"
>      "name": "Option B"
>}
>```

>예시 92
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Question",
>  "name": "무엇이 정답일까요?",
>  "anyOf": [
>    {
>      "type": "Note",
>      "name": "선택지 A"
>    },
>    {
>      "type": "Note",
>      "name": "선택지 B"
>    }
>  ]
>}
>```

#### [Class] [closed](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#closed`
Notes: | Indicates that a question has been closed, and answers are no longer accepted.
Domain: | [Question](ActivityVocabularyChapter3.md#class-question)
Range: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link) \| `xsd:dateTime` \| `xsd:boolean`

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#closed`
비고: | 질문이 마감(closed)되었으며, 더 이상 답변을 받지 않음을 나타냅니다.
도메인: | [Question](ActivityVocabularyChapter3.md#class-question)
범위: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link) \| `xsd:dateTime` \| `xsd:boolean`

>Example 93
>
>```json
>{
>  "name": "What is the answer?",
>}
>```

>예시 93
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Question",
>  "name": "무엇이 정답일까요?",
>  "closed": "2016-05-10T00:00:00Z"
>}
>```

#### [Class] [origin](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#origin`
Notes: | Describes an indirect object of the activity from which the activity is directed. The precise meaning of the origin is the object of the English preposition "from". For instance, in the activity "John moved an item to List B from List A", the origin of the activity is "List A".
Domain: | [Activity](ActivityVocabularyChapter2.md#class-activity)
Range: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#origin`
비고: | 액티비티가 지시하는 액티비티의 간접적인 객체를 표현합니다. 원산지(origin)의 정확한 의미는 영어 전치사 "from"의 목적 입니다. 예를 들어, "John이 품목을 리스트A 에서 리스트B로 옮겼습니다" 액티비티에서 액티비티의 원산지는 "리스트A" 입니다.
도메인: | [Activity](ActivityVocabularyChapter2.md#class-activity)
범위: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

[//Comment]: # "번역이 매끄럽지 않은것 같습니다"

>Example 94
>
>```json
>{
>  "summary": "Sally moved a post from List A to List B",
>    "name": "List B"
>    "name": "List A"
>}
>```

>예시 94
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally는 리스트 A에서 리스트 B로 게시물을 옮겼습니다.",
>  "type": "Move",
>  "actor": "http://sally.example.org",
>  "object": "http://example.org/posts/1",
>  "target": {
>    "type": "Collection",
>    "name": "리스트 B"
>  },
>  "origin": {
>    "type": "Collection",
>    "name": "리스트 A"
>  }
>}
>```

#### [Class] [next](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#next`
Notes: | In a paged [Collection](ActivityVocabularyChapter2.md#class-collection), indicates the next page of items.
Domain: | [CollectionPage](ActivityVocabularyChapter2.md#class-collectionpage)
Range: | [CollectionPage](ActivityVocabularyChapter2.md#class-collectionpage) \| [Link](ActivityVocabularyChapter2.md#class-link)
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#next`
비고: | 페이징 된 [Collection](ActivityVocabularyChapter2.md#class-collection)에서 항목들의 다음(next) 페이지를 나타냅니다.
도메인: | [CollectionPage](ActivityVocabularyChapter2.md#class-collectionpage)
범위: | [CollectionPage](ActivityVocabularyChapter2.md#class-collectionpage) \| [Link](ActivityVocabularyChapter2.md#class-link)
기능적: | True

>Example 95
>
>```json
>{
>  "summary": "Page 2 of Sally's blog posts",
>}
>```

>예시 95
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally의 블로그 포스트 2 페이지",
>  "type": "CollectionPage",
>  "next": "http://example.org/collection?page=2",
>  "items": [
>    "http://example.org/posts/1",
>    "http://example.org/posts/2",
>    "http://example.org/posts/3"
>  ]
>}
>```

>Example 96
>
>```json
>{
>  "summary": "Page 2 of Sally's blog posts",
>    "name": "Next Page",
>}
>```

>예시 96
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally의 블로그 포스트 2 페이지",
>  "type": "CollectionPage",
>  "next": {
>    "type": "Link",
>    "name": "다음 페이지",
>    "href": "http://example.org/collection?page=2"
>  },
>  "items": [
>    "http://example.org/posts/1",
>    "http://example.org/posts/2",
>    "http://example.org/posts/3"
>  ]
>}
>```

#### [Class] [object](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#object`
Notes: | When used within an [Activity](ActivityVocabularyChapter2.md#class-activity), describes the direct object of the activity. For instance, in the activity "John added a movie to his wishlist", the object of the activity is the movie added.</br> When used within a [Relationship](#class-relationship) describes the entity to which the [subject](#class-subject) is related.
Domain: | [Activity](ActivityVocabularyChapter2.md#class-activity) \| [Relationship](#class-relationship)
Range: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#object`
비고: | [Activity](ActivityVocabularyChapter2.md#class-activity) 내에서 사용될 경우, 액티비티의 직접적인 대상인 객체(object)를 설명합니다. 예를 들어 "John이 자신의 위시리스트에 영화를 추가했습니다" 액티비티에서 액티비티의 객체는 추가된 영화입니다. </br> [Relationship](#class-relationship) 내에서 사용될 경우 [subject](#class-subject)와 관련된 개체를 설명합니다.
도메인: | [Activity](ActivityVocabularyChapter2.md#class-activity) \| [Relationship](#class-relationship)
범위: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

>Example 97
>
>```json
>{
>  "summary": "Sally liked a post",
>}
>```

>예시 97
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally가 게시물을 좋아했습니다",
>  "type": "Like",
>  "actor": "http://sally.example.org",
>  "object": "http://example.org/posts/1"
>}
>```

[//Comment]: # "번역이 매끄럽지 않은것 같습니다."

>Example 98
>
>```json
>{
>    "content": "A simple note"
>}
>```

>예시 98
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Like",
>  "actor": "http://sally.example.org",
>  "object": {
>    "type": "Note",
>    "content": "간단한 노트"
>  }
>}
>```

>Example 99
>
>```json
>{
>  "summary": "Sally liked a note",
>      "summary": "A simple note",
>      "content": "That is a tree."
>}
>```

>예시 99
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally가 게시물을 좋아했습니다",
>  "type": "Like",
>  "actor": "http://sally.example.org",
>  "object": [
>    "http://example.org/posts/1",
>    {
>      "type": "Note",
>      "summary": "간단한 노트",
>      "content": "저건 나무야."
>    }
>  ]
>}
>```

#### [Class] [prev](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#prev`
Notes: | In a paged [Collection](ActivityVocabularyChapter2.md#class-collection), identifies the previous page of items.
Domain: | [CollectionPage](ActivityVocabularyChapter2.md#class-collectionpage)
Range: | [CollectionPage](ActivityVocabularyChapter2.md#class-collectionpage) \| [Link](ActivityVocabularyChapter2.md#class-link)
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#prev`
비고: | 페이징 된 [Collection](ActivityVocabularyChapter2.md#class-collection)에서 항목들의 이전(previous) 페이지를 식별합니다.
도메인: | [CollectionPage](ActivityVocabularyChapter2.md#class-collectionpage)
범위: | [CollectionPage](ActivityVocabularyChapter2.md#class-collectionpage) \| [Link](ActivityVocabularyChapter2.md#class-link)
기능적: | True

>Example 100
>
>```json
>{
>  "summary": "Page 1 of Sally's blog posts",
>}
>```

>예시 100
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally의 블로그 게시물 1 페이지",
>  "type": "CollectionPage",
>  "prev": "http://example.org/collection?page=1",
>  "items": [
>    "http://example.org/posts/1",
>    "http://example.org/posts/2",
>    "http://example.org/posts/3"
>  ]
>}
>```

>Example 101
>
>```json
>{
>  "summary": "Page 1 of Sally's blog posts",
>    "name": "Previous Page",
>}
>```

>예시 101
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally의 블로그 게시물 1 페이지",
>  "type": "CollectionPage",
>  "prev": {
>    "type": "Link",
>    "name": "이전 페이지",
>    "href": "http://example.org/collection?page=1"
>  },
>  "items": [
>    "http://example.org/posts/1",
>    "http://example.org/posts/2",
>    "http://example.org/posts/3"
>  ]
>}
>```

#### [Class] [preview](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#preview`
Notes: | Identifies an entity that provides a preview of this object.
Domain: | [Link](ActivityVocabularyChapter2.md#class-link) \| [Object](ActivityVocabularyChapter2.md#class-object)
Range: | [Link](ActivityVocabularyChapter2.md#class-link) \| [Object](ActivityVocabularyChapter2.md#class-object)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#preview`
비고: | 이 객체의 미리보기(preview)를 제공하는 개체를 식별합니다.
도메인: | [Link](ActivityVocabularyChapter2.md#class-link) \| [Object](ActivityVocabularyChapter2.md#class-object)
범위: | [Link](ActivityVocabularyChapter2.md#class-link) \| [Object](ActivityVocabularyChapter2.md#class-object)

>Example 102
>
>```json
>{
>  "name": "Cool New Movie",
>    "name": "Trailer",
>}
>```

>예시 102
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Video",
>  "name": "멋진 새 영화",
>  "duration": "PT2H30M",
>  "preview": {
>    "type": "Video",
>    "name": "예고편",
>    "duration": "PT1M",
>    "url": {
>      "href": "http://example.org/trailer.mkv",
>      "mediaType": "video/mkv"
>    }
>  }
>}
>```

#### [Class] [result](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#result`
Notes: | Describes the result of the activity. For instance, if a particular action results in the creation of a new resource, the result property can be used to describe that new resource.
Domain: | [Activity](ActivityVocabularyChapter2.md#class-activity)
Range: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#result`
비고: | 액티비티의 결과(result)를 표현합니다. 예를 들어, 특정 작업으로 인해 새 리소스가 생성되면 result 속성을 사용하여 해당 새 리소스를 표현할 수 있습니다.
도메인: | [Activity](ActivityVocabularyChapter2.md#class-activity)
범위: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

>Example 103
>
>```json
>{
>  "summary": "Sally checked that her flight was on time",
>    "name": "On Time"
>}
>```

>예시 103
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally는 비행기가 정시에 도착했는지 확인했습니다",
>  "type": ["Activity", "http://www.verbs.example/Check"],
>  "actor": "http://sally.example.org",
>  "object": "http://example.org/flights/1",
>  "result": {
>    "type": "http://www.types.example/flightstatus",
>    "name": "정시 도착"
>  }
>}
>```

#### [Class] [replies](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#replies`
Notes: | Identifies a [Collection](ActivityVocabularyChapter2.md#class-collection) containing objects considered to be responses to this object.
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | [Collection](ActivityVocabularyChapter2.md#class-collection)
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#replies`
비고: | 이 객체에 대한 응답으로 간주되는 객체가 포함된 [Collection](ActivityVocabularyChapter2.md#class-collection)을 식별합니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | [Collection](ActivityVocabularyChapter2.md#class-collection)
기능적: | True

>Example 104
>
>```json
>{
>  "summary": "A simple note",
>  "content": "I am fine.",
>        "summary": "A response to the note",
>        "content": "I am glad to hear it.",
>}
>```

>예시 104
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "간단한 노트",
>  "type": "Note",
>  "id": "http://www.test.example/notes/1",
>  "content": "전 괜찮아요.",
>  "replies": {
>    "type": "Collection",
>    "totalItems": 1,
>    "items": [
>      {
>        "summary": "노트에 대한 답장",
>        "type": "Note",
>        "content": "정말 다행이네요.",
>        "inReplyTo": "http://www.test.example/notes/1"
>      }
>    ]
>  }
>}
>```

#### [Class] [tag](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#tag`
Notes: | One or more "tags" that have been associated with an objects. A tag can be any kind of Object. The key difference between `attachment` and `tag` is that the former implies association by inclusion, while the latter implies associated by reference.
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#tag`
비고: | 개체와 관련된 하나 이상의 "태그들(tags)"입니다. 태그는 모든 종류의 Object일수 있습니다. `attachment`과 `tag`의 주요 차이점은 전자는 포함에 의한 연관을 의미하고, 후자는 참조에 의해 연관됨을 의미합니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

>Example 105
>
>```json
>{
>  "summary": "Picture of Sally",
>}
>```

>예시 105
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Image",
>  "summary": "Sally의 사진",
>  "url": "http://example.org/sally.jpg",
>  "tag": [
>    {
>      "type": "Person",
>      "id": "http://sally.example.org",
>      "name": "Sally"
>    }
>  ]
>}
>```

#### [Class] [target](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#target`
Notes: | Describes the indirect object, or target, of the activity. The precise meaning of the target is largely dependent on the type of action being described but will often be the object of the English preposition "to". For instance, in the activity "John added a movie to his wishlist", the target of the activity is John's wishlist. An activity can have more than one target.
Domain: | [Activity](ActivityVocabularyChapter2.md#class-activity)
Range: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#target`
비고: | 액티비티의 간접 객체 또는 대상(target)을 설명합니다. target의 정확한 의미는 표현하고 있는 작업 유형에 따라 크게 달라지지만, 종종 영어 전치사 "to"의 대상이 됩니다. 예를 들어, "John이 자신의 위시리스트에 영화를 추가했습니다" 액티비티에서 이 액티비티의 target은 John의 위시리스트 입니다. 액티비티에는 둘 이상의 target이 있을수도 있습니다.
도메인: | [Activity](ActivityVocabularyChapter2.md#class-activity)
범위: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

>Example 106
>
>```json
>{
>  "summary": "Sally offered the post to John",
>}
>```


>예시 106
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally는 John에게 게시물을 제공했습니다",
>  "type": "Offer",
>  "actor": "http://sally.example.org",
>  "object": "http://example.org/posts/1",
>  "target": "http://john.example.org"
>}
>```

>Example 107
>
>```json
>{
>  "summary": "Sally offered the post to John",
>}
>```

>예시 107
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally는 John에게 그 게시물을 제공했습니다",
>  "type": "Offer",
>  "actor": "http://sally.example.org",
>  "object": "http://example.org/posts/1",
>  "target": {
>    "type": "Person",
>    "name": "John"
>  }
>}
>```

#### [Class] [to](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#to`
Notes: | Identifies an entity considered to be part of the public primary audience of an Object
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#to`
비고: | 객체의 공개 주요 대상의 일부로 간주되는 개체를 식별합니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)

>Example 108
>
>```json
>{
>  "summary": "Sally offered the post to John",
>}
>```

>예시 108
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally는 John에게 그 게시물을 제공했습니다",
>  "type": "Offer",
>  "actor": "http://sally.example.org",
>  "object": "http://example.org/posts/1",
>  "target": "http://john.example.org",
>  "to": [ "http://joe.example.org" ]
>}
>```

#### [Class] [url](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#url`
Notes: | Identifies one or more links to representations of the object
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | `xsd:anyURI` \| [Link](ActivityVocabularyChapter2.md#class-link)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#url`
비고: | 객체 표현에 대한 하나 이상의 링크를 식별합니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | `xsd:anyURI` \| [Link](ActivityVocabularyChapter2.md#class-link)

>Example 109
>
>```json
>{
>  "name": "4Q Sales Forecast",
>}
>```

>예시 109
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Document",
>  "name": "4분기 판매 동향",
>  "url": "http://example.org/4q-sales-forecast.pdf"
>}
>```

>Example 110
>
>```json
>{
>  "name": "4Q Sales Forecast",
>}
>```

>예시 110
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Document",
>  "name": "4분기 판매 동향",
>  "url": {
>    "type": "Link",
>    "href": "http://example.org/4q-sales-forecast.pdf"
>  }
>}
>```

>Example 111
>
>```json
>{
>  "name": "4Q Sales Forecast",
>}
>```

>예시 111
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Document",
>  "name": "4분기 판매 동향",
>  "url": [
>    {
>      "type": "Link",
>      "href": "http://example.org/4q-sales-forecast.pdf",
>      "mediaType": "application/pdf"
>    },
>    {
>      "type": "Link",
>      "href": "http://example.org/4q-sales-forecast.html",
>      "mediaType": "text/html"
>    }
>  ]
>}
>```

#### [Class] [accuracy](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#accuracy`
Notes: | Indicates the accuracy of position coordinates on a [Place](ActivityVocabularyChapter3.md#class-place) objects. Expressed in properties of percentage. e.g. "94.0" means "94.0% accurate".
Domain: | [Place](ActivityVocabularyChapter3.md#class-place)
Range: | `xsd:float` [>= 0.0f, <= 100.0f]
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#accuracy`
비고: | [Place](ActivityVocabularyChapter3.md#class-place) 객체에서 위치 좌표의 정확도(accuracy)를 나타냅니다. 백분율 속성으로 표현됩니다. 예: "94.0"은 "94.0% 정확도"를 의미합니다.
도메인: | [Place](ActivityVocabularyChapter3.md#class-place)
범위: | `xsd:float` [>= 0.0f, <= 100.0f]
기능적: | True

>Example 112
>
>```json
>{
>  "name": "Liu Gu Lu Cun, Pingdu, Qingdao, Shandong, China",
>}
>```

>예시 112
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "name": "류구루촌, 핑두시, 칭다오시, 산둥성, 중국",
>  "type": "Place",
>  "latitude": 36.75,
>  "longitude": 119.7667,
>  "accuracy": 94.5
>}
>```

#### [Class] [altitude](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#altitude`
Notes: | Indicates the altitude of a place. The measurement units is indicated using the [units](#class-units) property. If [units](#class-units) is not specified, the default is assumed to be "`m`" indicating meters.
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | `xsd:float`
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#altitude`
비고: | 장소의 고도(altitude)를 나타냅니다. 측정 단위(units)는 [units](#class-units) 속성을 사용하여 표시됩니다. [units](#class-units)가 지정되지 않은 경우, 기본값은 미터를 나타내는 "`m`"으로 가정됩니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | `xsd:float`
기능적: | True

>Example 113
>
>```json
>{
>  "name": "Fresno Area",
>}
>```

>예시 113
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Place",
>  "name": "Fresno 지역",
>  "altitude": 15.0,
>  "latitude": 36.75,
>  "longitude": 119.7667,
>  "units": "miles"
>}
>```

#### [Class] [content](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#content`
Notes: | The content or textual representation of the Object encoded as a JSON string. By default, the value of `content` is HTML. The [mediaType](#class-mediatype) property can be used in the object to indicate a different content type. </br> The content *MAY* be expressed using multiple language-tagged values.
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | `xsd:string` \| `rdf:langString`

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#content`
비고: | JSON 문자열로 인코딩된 객체(Object)의 컨텐츠(content) 또는 텍스트 표현입니다. 기본적으로 `content`의 값은 HTML입니다. [mediaType](#class-mediatype) 속성을 객체에서 사용하여 다른 내용 유형을 나타낼 수 있습니다. </br> 컨텐츠는 여러 언어 태그값을 사용하여 표현될 수 있습니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | `xsd:string` \| `rdf:langString`

>Example 114
>
>```json
>{
>  "summary": "A simple note",
>  "content": "A <em>simple</em> note"
>}
>```

>예시 114
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "간단한 노트",
>  "type": "Note",
>  "content": "<em>간단한</em> 노트"
>}
>```

>Example 115
>
>```json
>{
>  "summary": "A simple note",
>}
>```

>예시 115
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "간단한 노트",
>  "type": "Note",
>  "contentMap": {
>    "en": "A <em>simple</em> note",
>    "es": "Una nota <em>sencilla</em>",
>    "zh-Hans": "一段<em>简单的</em>笔记"
>  }
>}
>```

>Example 116
>
>```json
>{
>  "summary": "A simple note",
>  "content": "## A simple note\nA simple markdown `note`"
>}
>```

>예시 116
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "간단한 노트",
>  "type": "Note",
>  "mediaType": "text/markdown",
>  "content": "## 간단한 노트\n간단한 마크다운 `노트`"
>}
>```

#### [Class] [name](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#name`
Notes: | A simple, human-readable, plain-text name for the object. HTML markup *MUST NOT* be included. The name *MAY* be expressed using multiple language-tagged values.
Domain: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)
Range: | `xsd:string` \| `rdf:langString`

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#name`
비고: | 간단하고 사람이 읽을수 있는 객체의 일반 텍스트 이름(name)입니다. HTML 마크업을 포함하는 것을 *절대 하지 말아야* 합니다. name은 여러 언어 태그 값을 사용하여 표현 *할 수도* 있습니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object) \| [Link](ActivityVocabularyChapter2.md#class-link)
범위: | `xsd:string` \| `rdf:langString`

>Example 117
>
>```json
>{
>  "name": "A simple note"
>}
>```

>예시 117
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Note",
>  "name": "간단한 노트"
>}
>```

>Example 118

>예시 118
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Note",
>  "nameMap": {
>    "en": "A simple note",
>    "es": "Una nota sencilla",
>    "zh-Hans": "一段简单的笔记"
>  }
>}
>```

#### [Class] [duration](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#duration`
Notes: | When the object describes a time-bound resource, such as an audio or video, a meeting, etc, the [duration](#class-duration) property indicates the object's approximate duration. The value *MUST* be expressed as an `xsd:duration` as defined by [ [xmlschema11-2](ActivityVocabularyChapterC.md#xmlschema11-2)], section 3.3.6 (e.g. a period of 5 seconds is represented as "`PT5S`").
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | `xsd:duration`
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#duration`
비고: | 객체가 오디오 또는 비디오, 회의등과 같은 시간 제한 리소스를 설명할떄 [duration](#class-duration) 속성은 객체의 대략적인 지속(duration) 시간을 나타냅니다. 값은 [ [xmlschema11-2](ActivityVocabularyChapterC.md#xmlschema11-2)], 섹션 3.3.6에 정의된 `xsd:duration`으로 표현되어야 합니다 (예: 5초 주기는 "`PT5S`"로 표기).
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | `xsd:duration`
기능적: | True

>Example 119
>
>```json
>{
>  "name": "Birds Flying",
>}
>```

>예시 119
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Video",
>  "name": "새들이 날라다님",
>  "url": "http://example.org/video.mkv",
>  "duration": "PT2H"
>}
>```

#### [Class] [height](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#height`
Notes: | On a [Link](ActivityVocabularyChapter2.md#class-link), specifies a hint as to the rendering height in device-independent pixels of the linked resource.
Domain: | [Link](ActivityVocabularyChapter2.md#class-link)
Range: | `xsd:nonNegativeInteger`
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#height`
비고: | [Link](ActivityVocabularyChapter2.md#class-link)에서 링크된 리소스의 장치 독립적 픽셀의 렌더링 높이(height)에 대한 힌트를 지정합니다.
도메인: | [Link](ActivityVocabularyChapter2.md#class-link)
범위: | `xsd:nonNegativeInteger`
기능적: | True

>Example 120

>예시 120
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Link",
>  "href": "http://example.org/image.png",
>  "height": 100,
>  "width": 100
>}
>```

#### [Class] [href](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#href`
Notes: | The target resource pointed to by a [Link](ActivityVocabularyChapter2.md#class-link).
Domain: | [Link](ActivityVocabularyChapter2.md#class-link)
Range: | `xsd:anyURI`
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#href`
비고: | [Link](ActivityVocabularyChapter2.md#class-link)가 가리키는 대상 자원입니다.
도메인: | [Link](ActivityVocabularyChapter2.md#class-link)
범위: | `xsd:anyURI`
기능적: | True

>Example 121
>
>```json
>{
>  "name": "Previous"
>}
>```

>예시 121
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Link",
>  "href": "http://example.org/abc",
>  "mediaType": "text/html",
>  "name": "이전"
>}
>```

#### [Class] [hreflang](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#hreflang`
Notes: | Hints as to the language used by the target resource. Value *MUST* be a [[BCP47](ActivityVocabularyChapterC.md#BCP47)] Language-Tag.
Domain: | [Link](ActivityVocabularyChapter2.md#class-link)
Range: | [[BCP47](ActivityVocabularyChapterC.md#BCP47)] Language Tag
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#hreflang`
비고: | 대상 자원이 사용하는 언어에 대한 힌트입니다. 값은 *반드시* [[BCP47](ActivityVocabularyChapterC.md#BCP47)] 언어 태그여야 합니다.
도메인: | [Link](ActivityVocabularyChapter2.md#class-link)
범위: | [[BCP47](ActivityVocabularyChapterC.md#BCP47)] 언어 태그
기능적: | True

>Example 122
>
>```json
>{
>  "name": "Previous"
>}
>```

>예시 122
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Link",
>  "href": "http://example.org/abc",
>  "hreflang": "en",
>  "mediaType": "text/html",
>  "name": "이전"
>}
>```

#### [Class] [partOf](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#partOf`
Notes: | Identifies the [Collection](ActivityVocabularyChapter2.md#class-collection) to which a [CollectionPage](ActivityVocabularyChapter2.md#class-collectionpage) objects items belong.
Domain: | [CollectionPage](ActivityVocabularyChapter2.md#class-collectionpage)
Range: | [Link](ActivityVocabularyChapter2.md#class-link) \| [Collection](ActivityVocabularyChapter2.md#class-collection)
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#partOf`
비고: | [CollectionPage](ActivityVocabularyChapter2.md#class-collectionpage) 객체 항목이 속하는 [Collection](ActivityVocabularyChapter2.md#class-collection)을 식별합니다.
도메인: | [CollectionPage](ActivityVocabularyChapter2.md#class-collectionpage)
범위: | [Link](ActivityVocabularyChapter2.md#class-link) \| [Collection](ActivityVocabularyChapter2.md#class-collection)
기능적: | True

>Example 123
>
>```json
>{
>  "summary": "Page 1 of Sally's notes",
>      "name": "Pizza Toppings to Try"
>      "name": "Thought about California"
>}
>```

>예시 123
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally의 노트 1 페이지",
>  "type": "CollectionPage",
>  "id": "http://example.org/collection?page=1",
>  "partOf": "http://example.org/collection",
>  "items": [
>    {
>      "type": "Note",
>      "name": "시도해볼 피자 토핑"
>    },
>    {
>      "type": "Note",
>      "name": "캘리포니아에 대한 생각"
>    }
>  ]
>}
>```

#### [Class] [latitude](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#latitude`
Notes: | The latitude of a place
Domain: | [Place](ActivityVocabularyChapter3.md#class-place)
Range: | `xsd:float`
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#latitude`
비고: | 장소의 위도(latitude)를 표시합니다.
도메인: | [Place](ActivityVocabularyChapter3.md#class-place)
범위: | `xsd:float`
기능적: | True

>Example 124
>
>```json
>{
>  "name": "Fresno Area",
>}
>```

>예시 124
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Place",
>  "name": "Fresno 지역",
>  "latitude": 36.75,
>  "longitude": 119.7667,
>  "radius": 15,
>  "units": "miles"
>}
>```

#### [Class] [longitude](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#longitude`
Notes: | The longitude of a place
Domain: | [Place](ActivityVocabularyChapter3.md#class-place)
Range: | `xsd:float`
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#longitude`
비고: | 장소의 경도(longitude)를 표시합니다.
도메인: | [Place](ActivityVocabularyChapter3.md#class-place)
범위: | `xsd:float`
기능적: | True

>Example 125
>
>```json
>{
>  "name": "Fresno Area",
>}
>```

>예시 125
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Place",
>  "name": "Fresno 지역",
>  "latitude": 36.75,
>  "longitude": 119.7667,
>  "radius": 15,
>  "units": "miles"
>}
>```

#### [Class] [mediaType](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#mediaType`
Notes: | When used on a [Link](ActivityVocabularyChapter2.md#class-link), identifies the MIME media type of the referenced resource. </br> When used on an [Object](ActivityVocabularyChapter2.md#class-object), identifies the MIME media type of the value of the [content](#class-content) property. If not specified, the [content](#class-content) property is assumed to contain `text/html` content.
Domain: | [Link](ActivityVocabularyChapter2.md#class-link) \| [Object](ActivityVocabularyChapter2.md#class-object)
Range: | MIME Media Type
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#mediaType`
비고: | [Link](ActivityVocabularyChapter2.md#class-link)에서 사용될 떄 참조된 리소스의 MIME 미디어 타입(media type)을 식별합니다. </br> [Object](ActivityVocabularyChapter2.md#class-object)에서 사용될 때 [content](#class-content) 속성 값의 MIME 미디어 유형을 식별합니다. 지정하지 않으면 [content](#class-content) 속성은 `text/html` 컨텐츠를 포함한다고 가정합니다.
도메인: | [Link](ActivityVocabularyChapter2.md#class-link) \| [Object](ActivityVocabularyChapter2.md#class-object)
범위: | MIME 미디어 타입
기능적: | True

>Example 126
>
>```json
>{
>  "name": "Next"
>}
>```

>예시 126
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Link",
>  "href": "http://example.org/abc",
>  "hreflang": "en",
>  "mediaType": "text/html",
>  "name": "다음"
>}
>```

#### [Class] [endTime](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#endTime`
Notes: | The date and time describing the actual or expected ending time of the object. When used with an [Activity](ActivityVocabularyChapter2.md#class-activity) object, for instance, the [endTime](#class-endtime) property specifies the moment the activity concluded or is expected to conclude.
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | `xsd:dateTime`
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#endTime`
비고: | 객체의 실제 또는 예상 종료 시간을 설명하는 날짜 및 시간입니다. 예를 들어, [Activity](ActivityVocabularyChapter2.md#class-activity) 객체와 함께 사용되는 경우 [endTime](#class-endtime) 속성은 액티비티가 종료되거나 종료 될것으로 예상되는 순간을 지정합니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | `xsd:dateTime`
기능적: | True

>Example 127
>
>```json
>{
>  "name": "Going-Away Party for Jim",
>}
>```

>예시 127
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Event",
>  "name": "Jim을 위한 송별회",
>  "startTime": "2014-12-31T23:00:00-08:00",
>  "endTime": "2015-01-01T06:00:00-08:00"
>}
>```

#### [Class] [published](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#published`
Notes: | The date and time at which the object was published
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | `xsd:dateTime`
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#published`
비고: | 개체가 게시된(published) 날짜와 시간입니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | `xsd:dateTime`
기능적: | True

>Example 128
>
>```json
>{
>  "summary": "A simple note",
>  "content": "Fish swim.",
>}
>```

>예시 128
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "간단한 노트",
>  "type": "Note",
>  "content": "물고기가 헤엄친다.",
>  "published": "2014-12-12T12:12:12Z"
>}
>```

#### [Class] [startTime](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#startTime`
Notes: | The date and time describing the actual or expected starting time of the object. When used with an [Activity](ActivityVocabularyChapter2.md#class-activity) object, for instance, the [startTime](#class-starttime) property specifies the moment the activity began or is scheduled to begin.
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | `xsd:dateTime`
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#startTime`
비고: | 객체의 실제 또는 예상 시작 시간(starting time)을 설명하는 날짜 및 시간입니다. 예를 들어, [Activity](ActivityVocabularyChapter2.md#class-activity) 객체와 함께 사용되는 경우 [startTime](#class-starttime) 속성은 액티비티가 시작되거나 예정된 순간을 지정합니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | `xsd:dateTime`
기능적: | True

>Example 129
>
>```json
>{
>  "name": "Going-Away Party for Jim",
>}
>```

>예시 129
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Event",
>  "name": "Jim을 위한 송별회",
>  "startTime": "2014-12-31T23:00:00-08:00",
>  "endTime": "2015-01-01T06:00:00-08:00"
>}
>```

#### [Class] [radius](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#radius`
Notes: | The radius from the given latitude and longitude for a Place. The units is expressed by the [units](#class-units) property. If [units](#class-units) is not specified, the default is assumed to be "`m`" indicating "meters".
Domain: | [Place](ActivityVocabularyChapter3.md#class-place)
Range: | `xsd:float` [>= 0.0f]
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#radius`
비고: | 장소에 대해 주어진 위도와 경도의 반경(radius)입니다. 단위(units)는 [units](#class-units) 속성으로 표시됩니다. [units](#class-units)가 지정되지 않은 경우 기본값은 "meters"를 나타내는 "`m`"으로 가정됩니다.
도메인: | [Place](ActivityVocabularyChapter3.md#class-place)
범위: | `xsd:float` [>= 0.0f]
기능적: | True

>Example 130
>
>```json
>{
>  "name": "Fresno Area",
>}
>```

>예시 130
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Place",
>  "name": "Fresno 지역",
>  "latitude": 36.75,
>  "longitude": 119.7667,
>  "radius": 15,
>  "units": "miles"
>}
>```

#### [Class] [rel](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#rel`
Notes: | A link relation associated with a [Link](ActivityVocabularyChapter2.md#class-link). The value *MUST* conform to both the [HTML5](ActivityVocabularyChapterC.md#HTML5) and [RFC5988](ActivityVocabularyChapterC.md#RFC5988) "link relation" definitions. </br> In the [HTML5](ActivityVocabularyChapterC.md#HTML5), any string not containing the "space" U+0020, "tab" (U+0009), "LF" (U+000A), "FF" (U+000C), "CR" (U+000D) or "," (U+002C) characters can be used as a valid link relation.
Domain: | [Link](ActivityVocabularyChapter2.md#class-link)
Range: | [RFC5988](ActivityVocabularyChapterC.md#RFC5988) or [HTML5](ActivityVocabularyChapterC.md#HTML5) Link Relation

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#rel`
비고: | Link와 관련된 링크 관계(relation). [HTML5](ActivityVocabularyChapterC.md#HTML5)와 [RFC5988](ActivityVocabularyChapterC.md#RFC5988) "링크 관계" 정의를 *반드시* 둘 다 준수해야합니다. </br> [HTML5](ActivityVocabularyChapterC.md#HTML5)에서 "space" U+0020, "tab" (U+0009), "LF" (U+000A), "FF" (U+000C), "CR" (U+000D) 또는 "," (U+002C) 문자를 포함하고 있지 않은 문자열은 유효한 링크 관계로 사용할 수 있습니다.
도메인: | [Link](ActivityVocabularyChapter2.md#class-link)
범위: | [RFC5988](ActivityVocabularyChapterC.md#RFC5988) 또는 [HTML5](ActivityVocabularyChapterC.md#HTML5) Link 관계

>Example 131
>
>```json
>{
>  "name": "Preview",
>}
>```

>예시 131
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Link",
>  "href": "http://example.org/abc",
>  "hreflang": "en",
>  "mediaType": "text/html",
>  "name": "미리보기",
>  "rel": ["canonical", "preview"]
>}
>```

#### [Class] [startIndex](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#startIndex`
Notes: | A non-negative integer value identifying the relative position within the logical view of a strictly ordered collection.
Domain: | [OrderedCollectionPage](ActivityVocabularyChapter2.md#class-orderedcollectionpage)
Range: | `xsd:nonNegativeInteger`
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#startIndex`
비고: | 엄격하게 정렬된 컬렉션의 논리적 뷰 내에서 상대 위치를 식별하는, 음이 아닌 정수의 값입니다.
도메인: | [OrderedCollectionPage](ActivityVocabularyChapter2.md#class-orderedcollectionpage)
범위: | `xsd:nonNegativeInteger`
기능적: | True

>Example 132
>
>```json
>{
>  "summary": "Page 1 of Sally's notes",
>      "name": "Density of Water"
>      "name": "Air Mattress Idea"
>}
>```

>예시 132
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Page 1 of Sally's notes",
>  "type": "OrderedCollectionPage",
>  "startIndex": 0,
>  "orderedItems": [
>    {
>      "type": "Note",
>      "name": "물의 밀도"
>    },
>    {
>      "type": "Note",
>      "name": "공기 매트리스 아이디어"
>    }
>  ]
>}
>```

#### [Class] [summary](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#summary`
Notes: | A natural language summarization of the object encoded as HTML. Multiple language tagged summaries *MAY* be provided.
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | `xsd:string` \| `rdf:langString`

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#summary`
비고: | HTML로 인코딩 된 객체의 자연어 요약(summary)입니다. 여러 언어 태그 요약이 제공 *될 수도* 있습니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | `xsd:string` \| `rdf:langString`

>Example 133
>
>```json
>{
>  "name": "Cane Sugar Processing",
>  "summary": "A simple <em>note</em>"
>}
>```

>예시 133
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "name": "사탕수수 가공",
>  "type": "Note",
>  "summary": "간단한 <em>노트</em>"
>}
>```

>Example 134
>
>```json
>{
>  "name": "Cane Sugar Processing",
>}
>```

>예시 134
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "name": "사탕수수 가공",
>  "type": "Note",
>  "summaryMap": {
>    "en": "A simple <em>note</em>",
>    "es": "Una <em>nota</em> sencilla",
>    "zh-Hans": "一段<em>简单的</em>笔记"
>  }
>}
>```

#### [Class] [totalItems](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#totalItems`
Notes: | A non-negative integer specifying the total number of objects contained by the logical view of the collection. This number might not reflect the actual number of items serialized within the [Collection](ActivityVocabularyChapter2.md#class-collection) object instance.
Domain: | [Collection](ActivityVocabularyChapter2.md#class-collection)
Range: | `xsd:nonNegativeInteger`
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#totalItems`
비고: | 컬렉션의 논리적 뷰에 포함된 총 개체수를 지정하는, 음이 아닌 정수입니다. 이 숫자는 [Collection](ActivityVocabularyChapter2.md#class-collection) 개체 인스턴스 내에서 직렬화된 실제 항목수를 반영하지 않을 수 있습니다.
도메인: | [Collection](ActivityVocabularyChapter2.md#class-collection)
범위: | `xsd:nonNegativeInteger`
기능적: | True

>Example 135
>
>```json
>{
>  "summary": "Sally's notes",
>      "name": "Which Staircase Should I Use"
>      "name": "Something to Remember"
>}
>```

>예시 135
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally의 노트",
>  "type": "Collection",
>  "totalItems": 2,
>  "items": [
>    {
>      "type": "Note",
>      "name": "어떤 계단을 사용해야 하지?"
>    },
>    {
>      "type": "Note",
>      "name": "기억해둬야 할것들"
>    }
>  ]
>}
>```

#### [Class] [units](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#units`
Notes: | Specifies the measurement units for the [radius](#class-radius) and [altitude](#class-altitude) properties on a [Place](ActivityVocabularyChapter3.md#class-place) object. If not specified, the default is assumed to be "`m`" for "meters".
Domain: | [Place](ActivityVocabularyChapter3.md#class-place)
Range: | "`cm`" \| " `feet`" \| " `inches`" \| " `km`" \| " `m`" \| " `miles`" \| `xsd:anyURI`
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#units`
비고: | [Place](ActivityVocabularyChapter3.md#class-place) 객체의 [radius](#class-radius) 및 [altitude](#class-altitude) 속성에 대한 측정 단위(units)를 지정합니다. 지정하지 않으면 기본값으로는 "미터"를 나타내는 "m"으로 간주됩니다.
도메인: | [Place](ActivityVocabularyChapter3.md#class-place)
범위: | "`cm`" \| " `feet`" \| " `inches`" \| " `km`" \| " `m`" \| " `miles`" \| `xsd:anyURI`
기능적: | True

>Example 136
>
>```json
>{
>  "name": "Fresno Area",
>}
>```

>예시 136
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Place",
>  "name": "Fresno 지역",
>  "latitude": 36.75,
>  "longitude": 119.7667,
>  "radius": 15,
>  "units": "miles"
>}
>```

#### [Class] [updated](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#updated`
Notes: | The date and time at which the object was updated
Domain: | [Object](ActivityVocabularyChapter2.md#class-object)
Range: | `xsd:dateTime`
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#updated`
비고: | 객체가 업데이트된(updated) 날짜 및 시간입니다.
도메인: | [Object](ActivityVocabularyChapter2.md#class-object)
범위: | `xsd:dateTime`
기능적: | True

>Example 137
>
>```json
>{
>  "name": "Cranberry Sauce Idea",
>  "content": "Mush it up so it does not have the same shape as the can.",
>}
>```

>예시 137
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "name": "크랜베리 소스 아이디어",
>  "type": "Note",
>  "content": "캔과 동일한 모양을 갖추지 않도록 위로 밀어 올리기.",
>  "updated": "2014-12-12T12:12:12Z"
>}
>```

#### [Class] [width](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#width`
Notes: | On a [Link](ActivityVocabularyChapter2.md#class-link), specifies a hint as to the rendering width in device-independent pixels of the linked resource.
Domain: | [Link](ActivityVocabularyChapter2.md#class-link)
Range: | `xsd:nonNegativeInteger`
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#width`
비고: | [Link](ActivityVocabularyChapter2.md#class-link)에서 링크된 리소스의 장치 독립적인 픽셀의 렌더링 너비(width)에 대한 힌트를 지정합니다.
도메인: | [Link](ActivityVocabularyChapter2.md#class-link)
범위: | `xsd:nonNegativeInteger`
기능적: | True

>Example 138

>예시 138
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "type": "Link",
>  "href": "http://example.org/image.png",
>  "height": 100,
>  "width": 100
>}
>```

#### [Class] [subject](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#subject`
Notes: | On a [Relationship](#class-relationship) object, the `subject` property identifies one of the connected individuals. For instance, for a Relationship object describing "John is related to Sally", `subject` would refer to John.
Domain: | [Relationship](#class-relationship)
Range: | [Link](ActivityVocabularyChapter2.md#class-link) \| [Object](ActivityVocabularyChapter2.md#class-object)
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#subject`
비고: | [Relationship](#class-relationship) 객체에서 `subject` 속성은 연결된 개개인중 한명을 식별합니다. 예를 들어, "John은 Sally와 관련이 있습니다"라는 관계 객체의 경우, `subject`는 John을 나타냅니다.
도메인: | [Relationship](#class-relationship)
범위: | [Link](ActivityVocabularyChapter2.md#class-link) \| [Object](ActivityVocabularyChapter2.md#class-object)
기능적: | True

>Example 139
>
>```json
>{
>  "summary": "Sally is an acquaintance of John's",
>}
>```

>예시 139
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally는 John의 지인입니다.",
>  "type": "Relationship",
>  "subject": {
>    "type": "Person",
>    "name": "Sally"
>  },
>  "relationship": "http://purl.org/vocab/relationship/acquaintanceOf",
>  "object": {
>    "type": "Person",
>    "name": "John"
>  }
>}
>```

#### [Class] [relationship](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#relationship`
Notes: | On a [Relationship](#class-relationship) object, the `relationship` property identifies the kind of relationship that exists between [subject](#class-subject) and [object](ActivityVocabularyChapter2.md#class-object).
Domain: | [Relationship](#class-relationship)
Range: | [Object](ActivityVocabularyChapter2.md#class-object)

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#relationship`
비고: | [Relationship](#class-relationship) 객체에서 `relationship` 속성은 [subject](#class-subject)와 [object](ActivityVocabularyChapter2.md#class-object) 사이에 존재하는 관계의 종류를 식별합니다.
도메인: | [Relationship](#class-relationship)
범위: | Object

>Example 140
>
>```json
>{
>  "summary": "Sally is an acquaintance of John's",
>}
>```

>예시 140
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally는 John의 지인입니다.",
>  "type": "Relationship",
>  "subject": {
>    "type": "Person",
>    "name": "Sally"
>  },
>  "relationship": "http://purl.org/vocab/relationship/acquaintanceOf",
>  "object": {
>    "type": "Person",
>    "name": "John"
>  }
>}
>```

#### [Class] [describes](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#describes`
Notes: | On a [Profile](#class-profile) object, the `describes` property identifies the object described by the Profile.
Domain: | [Profile](#class-profile)
Range: | [Object](ActivityVocabularyChapter2.md#class-object)
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#describes`
비고: | Profile 객체에서 `describes` 속성은 Profile이 설명(describes)하는 객체를 식별합니다.
도메인: | [Profile](#class-profile)
범위: | [Object](ActivityVocabularyChapter2.md#class-object)
기능적: | True

>Example 141
>
>```json
>{
>  "summary": "Sally's profile",
>}
>```

>예시 141
>
>```json
>{
>  "@context": "https://www.w3.org/ns/activitystreams",
>  "summary": "Sally의 프로필",
>  "type": "Profile",
>  "describes": {
>    "type": "Person",
>    "name": "Sally"
>  },
>  "url": "http://sally.example.org"
>}
>```

#### [Class] [formerType](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#formerType`
Notes: | On a [Tombstone](ActivityVocabularyChapter3.md#class-tombstone) object, the `formerType` property identifies the type of the object that was deleted.
Domain: | [Tombstone](ActivityVocabularyChapter3.md#class-tombstone)
Range: | [Object](ActivityVocabularyChapter2.md#class-object)
Functional: | False

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#formerType`
비고: | [Tombstone](ActivityVocabularyChapter3.md#class-tombstone) 객체에서 `formerType` 속성은 삭제된 객체의 타입을 식별합니다.
도메인: | [Tombstone](ActivityVocabularyChapter3.md#class-tombstone)
범위: | [Object](ActivityVocabularyChapter2.md#class-object)
기능적: | False

>Example 142
>
>```json
>{
>"summary": "This image has been deleted",
>}
>```

>예시 142
>
>```json
>{
>"@context": "https://www.w3.org/ns/activitystreams",
>"summary": "이 이미지는 삭제되었습니다",
>"type": "Tombstone",
>"formerType": "Image",
>"url": "http://example.org/image/2"
>}
>```

#### [Class] [deleted](#4-속성-properties)

Description| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#deleted`
Notes: | On a [Tombstone](ActivityVocabularyChapter3.md#class-tombstone) object, the `deleted` property is a timestamp for when the object was deleted.
Domain: | [Tombstone](ActivityVocabularyChapter3.md#class-tombstone)
Range: | `xsd:dateTime`
Functional: | True

설명| |
--|--
URI: | `https://www.w3.org/ns/activitystreams#deleted`
비고: | [Tombstone](ActivityVocabularyChapter3.md#class-tombstone) 객체에서 `deleted` 속성은 객체가 삭제(deleted)된 타임스탬프를 나타냅니다.
도메인: | [Tombstone](ActivityVocabularyChapter3.md#class-tombstone)
범위: | `xsd:dateTime`
기능적: | True

>Example 143
>
>```json
>{
>"summary": "This image has been deleted",
>}
>```

>예시 143
>
>```json
>{
>"@context": "https://www.w3.org/ns/activitystreams",
>"summary": "이 이미지는 삭제되었습니다",
>"type": "Tombstone",
>"deleted": "2016-05-03T00:00:00Z"
>}
>```

[맨 위로](#4-속성-properties)
