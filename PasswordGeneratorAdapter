// @ts-check
/* eslint-disable class-methods-use-this */

import generator from 'generate-password';

export default class PasswordGeneratorAdapter {
  generatePassword(length, options) {
    const init = { length, uppercase: false, numbers: false, symbols: false };
    const config = options.reduce((acc, curr) => ({...acc, [curr]: true}), init);
    return generator.generate(config);
  }
}
