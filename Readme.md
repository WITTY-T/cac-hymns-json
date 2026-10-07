# CAC Hymns JSON

A structured JSON collection of Christ Apostolic Church (CAC) hymns in English and Yoruba.

This repository is intended to make the hymn data easier for developers to use in applications such as church presentation software, hymn apps, worship applications, and other educational or church-related projects.

##  Available Datasets

| Dataset | File                    |
| ------- | ----------------------- |
| English | `data/cac_english.json` |
| Yoruba  | `data/cac_yoruba.json`  |

## JSON Structure

Each hymn follows a simple, consistent structure:

```json
{
  "id": "1150",
  "number": "V050",
  "metadata": "Ife gbogbo orilede yoo si de - Hag. 2:7",
  "category": "",
  "lyrics": "1. Gbo orin awon Angeli..."
}
```

### Fields

| Field      | Type   | Description                                   |
| ---------- | ------ | --------------------------------------------- |
| `id`       | string | Unique identifier for the hymn                |
| `number`   | string | Hymn number/reference                         |
| `metadata` | string | Additional information or scripture reference |
| `category` | string | Hymn category                                 |
| `lyrics`   | string | Complete hymn lyrics                          |

The `lyrics` field contains the complete text of the hymn, including numbered verses and any chorus or ending text included in the source data.


See [`schema.json`](schema.json) for the expected structure.

##  Using the Data

You can download the JSON files directly from this repository and load them into your application.

Example in JavaScript:

```js
const response = await fetch(
  "https://raw.githubusercontent.com/YOUR_USERNAME/cac-hymns-json/main/data/cac_english.json"
);

const hymns = await response.json();

console.log(hymns);
```

Replace `YOUR_USERNAME` with your GitHub username.

## 🌍 Languages

This repository currently contains:

* English hymns
* Yoruba hymns

More datasets may be added in the future.

## ⚠️ Attribution and Rights

The hymn texts contained in these datasets may be subject to copyright or other rights held by their respective authors, publishers, churches, or other rights holders.

This repository does not claim ownership of the original hymn texts.

The data is provided in a structured format for developers and projects that have the appropriate rights or permission to use the material.

Please verify the copyright and usage requirements applicable to the hymns before redistributing them or using them in a commercial application.

Where applicable, retain the original attribution and source information contained in the dataset.

## 🤝 Contributions

Contributions that improve the structure, consistency, documentation, or technical quality of the dataset are welcome.

Please avoid submitting copyrighted material unless you have the right to redistribute it.

## 📄 License

The repository's original code, schema, and documentation are licensed separately where applicable.

The hymn text itself is **not automatically licensed under the repository's software license** and remains subject to the rights of its respective copyright holders.
