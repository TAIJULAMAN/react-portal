A **React Portal** allows you to render children into a DOM node that exists outside the DOM hierarchy of the parent component. This is useful for cases where you want to break out of the normal flow of the DOM to render UI elements that may need to be visually above other elements, such as:

- **Modals**
- **Popups**
- **Tooltips**
- **Dropdowns**
- **Notifications**

### **How Portals Work in React:**

By default, React renders a component’s children inside the parent component’s DOM node. However, **with a portal**, you can render a component’s children into a different part of the DOM. This means that the component is logically part of the parent, but visually it can appear elsewhere.

### **Key Benefits of React Portals:**

1. **Breaking out of Overflow and Z-Index Issues**: A common use case is when you need a modal to appear on top of other content but the parent component has `overflow: hidden` or `z-index` restrictions.
2. **Managing Global UI Components**: For things like modals or tooltips, a portal allows you to manage these elements globally, outside of the parent component’s flow.
3. 

### **Why Use React Portals?**

1. **Z-Index and Layout Issues**: Components like modals or tooltips often need to break out of the constraints of their parent components. By rendering outside the parent hierarchy, a portal can avoid issues like clipping, `z-index` conflicts, or overflowing content.
2. **Global UI Elements**: Portals are perfect for elements like global notifications or alerts, where they need to be rendered outside the typical parent-child hierarchy but still be part of the component tree for logic and state management.
3. **Accessing DOM Directly**: Portals allow for direct access to the DOM, which might be necessary in some edge cases where you need to interact with elements that aren’t in the normal DOM flow.