<script>
export default {
	globalData: {
		userInformation: '',
		resultData: '',

		// 登入URL（H5端）
		loginUrl: {
			// url: '/api/User/Verify' //H5端
			url: 'http://www.sunagy.com:7000/User/Verify'	//APP端（测试）
			// url: 'http://api.sunagy.com/User/Verify'	//APP端（正试）
		},

		// flowMappingUrl: '/api/Apply/GetApplyFlowMappingByFlowID', //获取流程设计映射（H5）
		flowMappingUrl: 'http://www.sunagy.com:7000/Apply/GetApplyFlowMappingByFlowID',	//获取流程设计映射（APP测试）
		// flowMappingUrl: 'http://api.sunagy.com/Apply/GetApplyFlowMappingByFlowID',	//获取流程设计映射（APP正式）

		// getMappingUrl: '/api/Apply/GetApplyFlowObjectByMapping', //获取映射字段（H5）
		getMappingUrl: 'http://www.sunagy.com:7000/Apply/GetApplyFlowObjectByMapping'	,//获取映射字段（APP测试）
		// getMappingUrl: 'http://api.sunagy.com/Apply/GetApplyFlowObjectByMapping',	//获取映射字段（APP正式）

		// getFlowUrl: '/api/Apply/getApplyByIDAndValue', //获取某条申请流程的数据（H5）
		getFlowUrl: 'http://www.sunagy.com:7000/Apply/getApplyByIDAndValue', //获取某条申请流程的数据（APP测试）
		// getFlowUrl: 'http://api.sunagy.com/Apply/getApplyByIDAndValue', //获取某条申请流程的数据（APP正式）
		
		// getApplyListObjectByFlowID: '/api/Apply/GetApplyListObjectByFlowID', //获取关联流程的数据（H5）
		getApplyListObjectByFlowID: 'http://www.sunagy.com:7000/Apply/GetApplyListObjectByFlowID', //获取关联流程的数据（APP测试）
		// getApplyListObjectByFlowID: 'http://api.sunagy.com/Apply/GetApplyListObjectByFlowID', //获取关联流程的数据（APP正式）

		// submitApplyUrl: '/api/Apply/SubmitApply2', //提交用的URL（H5）
		submitApplyUrl: 'http://www.sunagy.com:7000/Apply/SubmitApply2',	//提交用的URL（APP测试）
		// submitApplyUrl: 'http://api.sunagy.com/Apply/SubmitApply2',	//提交用的URL（APP正式）
		
		
		// outWarehouseUrl: '/api/Apply/SubmitApply', //成品出库提交时的URL（H5）
		outWarehouseUrl: 'http://www.sunagy.com:7000/Apply/SubmitApply',	//成品出库提交时的URL（APP测试）
		// outWarehouseUrl: 'http://api.sunagy.com/Apply/SubmitApply',	//成品出库提交时的URL（APP正式）

		// submitModifyApplyUrl: '/api/Apply/ModifyApply', //重新编辑流程的URL（H5）
		submitModifyApplyUrl: 'http://www.sunagy.com:7000/Apply/ModifyApply', //重新编辑流程的URL（APP测试）
		// submitModifyApplyUrl: 'http://api.sunagy.com/Apply/ModifyApply', //重新编辑流程的URL（APP正式）

		// 首页需要的ID
		defaultData: {
			// 测试
			productWarehousing: '201906181336562572129213317409539126', //成品入库
			productOutStock: '202001101008013445409787075819036771', //成品出库
			productDiskEntry: '', //成品盘入
			productDishOut: '' //成品盘出

			// 正式
			// productWarehousing: '',	//成品入库
			// productOutStock: '',	//成品出库
			// productDiskEntry: '',	//成品盘入
			// productDishOut: '',	//成品盘出
		},

		//请求时需要的流程ID
		requestID: {
			//测试
			weekly_production_plan: '201908161508163702016565635121447867', //周生产计划
			finished_product_out_application: '201909140914551591210133789102548444', //成品出库申请单

			// 正式
			// weekly_production_plan: '',	//周生产计划
			// finished_product_warehousing: '',	//成品入库
		},

		pageUrl: {
			PWFlows: '../flows/PWFlows', // 成品入库页
			POFlows: '../flows/POFlows' // 成品出库页
		}
	},
	onLaunch: function() {
		console.log('App Launch');
	},
	onShow: function() {
		console.log('App Show');
	},
	onHide: function() {
		console.log('App Hide');
	}
};
</script>

<style>
/*每个页面公共css */
</style>
