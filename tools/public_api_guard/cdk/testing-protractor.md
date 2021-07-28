## API Report File for "components-srcs"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { ElementArrayFinder } from 'protractor';
import { ElementDimensions } from '@angular/cdk/testing';
import { ElementFinder } from 'protractor';
import { EventData } from '@angular/cdk/testing';
import { HarnessEnvironment } from '@angular/cdk/testing';
import { HarnessLoader } from '@angular/cdk/testing';
import { ModifierKeys } from '@angular/cdk/testing';
import { TestElement } from '@angular/cdk/testing';
import { TestKey } from '@angular/cdk/testing';
import { TextOptions } from '@angular/cdk/testing';

// @public @deprecated
export class ProtractorElement implements TestElement {
    constructor(element: ElementFinder);
    blur(): Promise<void>;
    clear(): Promise<void>;
    click(modifiers?: ModifierKeys): Promise<void>;
    click(location: 'center', modifiers?: ModifierKeys): Promise<void>;
    click(relativeX: number, relativeY: number, modifiers?: ModifierKeys): Promise<void>;
    dispatchEvent(name: string, data?: Record<string, EventData>): Promise<void>;
    // (undocumented)
    readonly element: ElementFinder;
    focus(): Promise<void>;
    getAttribute(name: string): Promise<string | null>;
    getCssValue(property: string): Promise<string>;
    getDimensions(): Promise<ElementDimensions>;
    getProperty<T = any>(name: string): Promise<T>;
    hasClass(name: string): Promise<boolean>;
    hover(): Promise<void>;
    isFocused(): Promise<boolean>;
    matchesSelector(selector: string): Promise<boolean>;
    mouseAway(): Promise<void>;
    rightClick(relativeX: number, relativeY: number, modifiers?: ModifierKeys): Promise<void>;
    selectOptions(...optionIndexes: number[]): Promise<void>;
    sendKeys(...keys: (string | TestKey)[]): Promise<void>;
    sendKeys(modifiers: ModifierKeys, ...keys: (string | TestKey)[]): Promise<void>;
    setInputValue(value: string): Promise<void>;
    text(options?: TextOptions): Promise<string>;
}

// @public @deprecated
export class ProtractorHarnessEnvironment extends HarnessEnvironment<ElementFinder> {
    protected constructor(rawRootElement: ElementFinder, options?: ProtractorHarnessEnvironmentOptions);
    protected createEnvironment(element: ElementFinder): HarnessEnvironment<ElementFinder>;
    protected createTestElement(element: ElementFinder): TestElement;
    forceStabilize(): Promise<void>;
    protected getAllRawElements(selector: string): Promise<ElementFinder[]>;
    protected getDocumentRoot(): ElementFinder;
    static getNativeElement(el: TestElement): ElementFinder;
    static loader(options?: ProtractorHarnessEnvironmentOptions): HarnessLoader;
    waitForTasksOutsideAngular(): Promise<void>;
}

// @public @deprecated
export interface ProtractorHarnessEnvironmentOptions {
    queryFn: (selector: string, root: ElementFinder) => ElementArrayFinder;
}

// (No @packageDocumentation comment for this package)

```