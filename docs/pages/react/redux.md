### Redux

**Redux**: State management tool/ library.

- When the application has lot of data management mechanism which required to be consistent among multiple areas or components ( i.e, all of them should use the same data)
- When passing data to deeply nested children is hard
  The above mentioned use cases are some areas we can use the redux which is immutable state (no modifications are allowed)

1. **Action**: specifies the logic in reducer to be executed.
1. **Reducer**: where the modification ( creation of new state) logic is handled.
1. **Store**: Which stores the data in read-only form.

**Advantages of using Redux**-

1. **Better Code Organization** – how the code needs to be organized. This results a code workable for any development team
1. **Developer Tools** – Allow developers to track each and everything.
1. Easy Testing
1. Maintainability
1. server-side rendering
