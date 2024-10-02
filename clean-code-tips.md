[Clean Code tip: Don't put types in your names.](https://www.linkedin.com/posts/danielmoka_clean-code-tip-dont-put-types-in-your-names-activity-7247123214915518464-ZDl7?utm_source=share&utm_medium=member_desktop)

It's redundant, it hurts readability and you need to change the name if the type changes

And most modern code editors display the types anyway.

Examples:

❌ productArray.addProduct
✅ cart.add(product)

❌ FileReaderInterfaceImpl
✅ FileReader

❌ userList | userArray | userItems | userCollection
✅ users

Write code for humans to read, not just for machines to execute.
