# @spudly/paginate

Determines which links to show for a pagination widget.

# Installation

```bash
npm install --save @spudly/paginate
```

# Usage

```js
import paginate from '@spudly/paginate';

const currentPage = 5;
const totalPages = 10;
const size = 3;

const pages = paginate(currentPage, totalPages, size);

// Result:
// [
//   {page: 0, type: 'FIRST', isCurrentPage: false},
//   {page: 4, type: 'PREV', isCurrentPage: false},
//   {page: 4, type: 'NUMBER', isCurrentPage: false},
//   {page: 5, type: 'NUMBER', isCurrentPage: true},
//   {page: 6, type: 'NUMBER', isCurrentPage: false},
//   {page: 6, type: 'NEXT', isCurrentPage: false},
//   {page: 9, type: 'LAST', isCurrentPage: false},
// ];
```
