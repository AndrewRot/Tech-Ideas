# Utility Creator

A browser plugin that helps you isolate web application tools & allow you to run them on their own.

Directory for existing 'isolated' tools. 

Open source it, so if a page updates, people can adjust how we isolate the tools.

### Ideas / Use cases
IE, Google has google translate built into their browser & still shows all over Google search results ont he page.
It would be cool to isolate just the HTML body used for that tool and create a nice little shell of a webapp that removes scrolling & other clutter on the page.

Data converters - like CVS ro XML or JSON. Just isolate the tool on the page and allow you to run them on their own without the rest of the page / ads


### Potential problems

If the tool communicates with external servers, you cannot extract / run the html/js on its own as the server may not accept requests coming in from another domain like localhost. 

The plugin could just render the tool itself, block / whiteout the rest of the html on the page. That way the requests come from the same domain.

### First steps

1.) Isolate the tool code on the page and see if you can run it on its own.
2.) Look around a bunch of tools to see how they work. 
   - Are they their own HTML / JS script
   - Do they require all the JS to run on the page?
3.) Is it difficult to remove all other parts of the html on the page?

Would have to be a tool that works on a per-domain basis
