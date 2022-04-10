# jp
const { writeConf } = require('@gh-conf/gh-conf-write');

(async () => {
  try {
    const writeResult = await writeConf('./gh-conf-write', 'CONTENT');
    console.log(writeResult);
    /**
     * {
     *   status: 'success',
     *   message: 'Config updated',
     *   data: {
     *       content: 'CONTENT'
     *   }
     * }
     **/
  } catch (error) {
    console.log(error);
  }
})();
