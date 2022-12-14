# Installation
> `npm install --save @types/object-inspect`

# Summary
This package contains type definitions for object-inspect (https://github.com/substack/object-inspect).

# Details
Files were exported from https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/types/object-inspect.
## [index.d.ts](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/types/object-inspect/index.d.ts)
````ts
// Type definitions for object-inspect 1.8
// Project: https://github.com/substack/object-inspect
// Definitions by: Charles Samborski <https://github.com/demurgos>
//                 Akuukis <https://github.com/Akuukis>
//                 Jordan Harband <https://github.com/ljharb>
// Definitions: https://github.com/DefinitelyTyped/DefinitelyTyped

declare namespace objectInspect {
    /**
     * Inspection options
     */
    interface Options {
        /**
         * Maximum depth of the inspection. Default: `5`.
         */
        depth?: number | undefined;
        /**
         * Must be "single" or "double", if present.
         */
        quoteStyle?: 'single' | 'double' | undefined;
        /**
         * Must be 0, a positive integer, Infinity, or null, if present. Default Infinity.
         */
        maxStringLength?: number | null | undefined;
        /**
         * When true, a custom inspect method function will be invoked. Default true.
         */
        customInspect?: boolean | undefined;
        /**
         * Must be "\t", null, or a positive integer. Default null.
         */
        indent?: number | '\t' | null | undefined;
    }
}

/**
 * Return a string `s` with the string representation of `obj` up to a depth of `opts.depth`.
 *
 * @param obj Object to inspect
 * @param opts Inspection options. Default: `{}`.
 * @return String representation of `obj`
 */
declare function objectInspect(obj: any, opts?: objectInspect.Options): string;

export = objectInspect;

````

### Additional Details
 * Last updated: Wed, 07 Jul 2021 16:31:36 GMT
 * Dependencies: none
 * Global values: none

# Credits
These definitions were written by [Charles Samborski](https://github.com/demurgos), [Akuukis](https://github.com/Akuukis), and [Jordan Harband](https://github.com/ljharb).
