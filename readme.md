    Server-side Rendering:

    Unlike a traditional React app where the entire application is loaded and rendered on the client,
    Next.js allows the first page load to be rendered by the server,
    which is great for Search Engine Optimization & performance

    React apps just load up the main div where everything is rendered and hence web crawlers
    cant pickup on that. This is handled by NextJS

    Routing is easier in NextJs. No need to use react-router-dom.

    create api routes within the next structure.

>> CSS
    all css files are stored in the styles folder.
    All files related to a component must have extension .module.css
    globals.css ==> has css for entire page

    >> style components
        we can import different css styles from the file add assign diffent tags classnames accordingly.
        import styles from '@/styles/globals.css'
        <div className={styles.div-t1}>...</div> ==> works in reverse fashion    

>> pages folder
    all the pages are stored here. The structuring of this folder defines the website structure

    -> _app.js ==> this file encompasses the entire rendered page. Here we import the gloal.css file.
    -> _document.js ==> dont make changes in this.
>> pages/api folder
    similar to express.

>> components vs pages --> pages may have components in them

>> if we run build = (npm next build && next export ) see package.json==> it generates a out folder which in itself can serve the static website created.  