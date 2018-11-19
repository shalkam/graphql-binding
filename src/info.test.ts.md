# Snapshot report for `src/info.test.ts`

The actual snapshot is saved in `info.test.ts.snap`.

Generated by [AVA](https://ava.li).

## makeSubInfo: works when path has been selected

> Snapshot 1

    `{␊
      content␊
      wordCount␊
    }␊
    `

> Snapshot 2

    {
      fieldName: 'page',
      fragments: {},
      operation: {
        kind: 'OperationDefinition',
        operation: 'page',
        selectionSet: {
          kind: 'SelectionSet',
          selections: [],
        },
        variableDefinitions: [],
      },
      parentType: 'Book',
      path: {
        key: 'page',
        prev: {
          key: 'book',
          prev: undefined,
        },
      },
      returnType: 'Page',
      rootValue: undefined,
      selectionSet: {
        kind: 'SelectionSet',
        selections: {
          0: {
            alias: undefined,
            arguments: {},
            directives: {},
            kind: 'Field',
            name: {
              kind: 'Name',
              value: 'content',
            },
            selectionSet: undefined,
          },
          1: {
            alias: undefined,
            arguments: {},
            directives: {},
            kind: 'Field',
            name: {
              kind: 'Name',
              value: 'wordCount',
            },
            selectionSet: undefined,
          },
        },
      },
      variableValues: {},
    }

## makeSubInfo: works when path has been selected and adds fragment

> Snapshot 1

    `{␊
      content␊
      wordCount␊
    }␊
    `

## makeSubInfo: works with inline fragment

> Snapshot 1

    `{␊
      page {␊
        content␊
      }␊
    }␊
    `

> Snapshot 2

    {
      fieldName: 'page',
      fragments: {},
      operation: {
        kind: 'OperationDefinition',
        operation: 'page',
        selectionSet: {
          kind: 'SelectionSet',
          selections: [],
        },
        variableDefinitions: [],
      },
      parentType: 'Book',
      path: {
        key: 'page',
        prev: {
          key: 'book',
          prev: undefined,
        },
      },
      returnType: 'Page',
      rootValue: undefined,
      selectionSet: {
        kind: 'SelectionSet',
        selections: {
          0: {
            alias: undefined,
            arguments: {},
            directives: {},
            kind: 'Field',
            name: {
              kind: 'Name',
              value: 'page',
            },
            selectionSet: {
              kind: 'SelectionSet',
              selections: {
                0: {
                  alias: undefined,
                  arguments: {},
                  directives: {},
                  kind: 'Field',
                  name: {
                    kind: 'Name',
                    value: 'content',
                  },
                  selectionSet: undefined,
                },
              },
            },
          },
        },
      },
      variableValues: {},
    }